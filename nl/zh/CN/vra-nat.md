---

copyright:
  years: 2017
lastupdated: "2018-11-10"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:download: .download}

# 将 NAT 与基于前缀的 IPsec 配合使用
在[为 VFP 接口配置 IPSec 和区域防火墙](vra-vfp.html)主题中，我们创建了一个 VFP 接口，并将其设置为用于 IPsec 隧道。 

我们可以在 NAT 规则中使用相同的接口，还可以使用入站和出站接口声明，但会有一个额外的警告。 

下面是一些示例 NAT 规则：

```
set service nat destination rule 10 destination address '172.16.200.2'
set service nat destination rule 10 inbound-interface 'vfp0'
set service nat destination rule 10 translation address '10.177.137.251'
set service nat source rule 10 outbound-interface 'vfp0'
set service nat source rule 10 source address '10.177.137.251'
set service nat source rule 10 translation address '172.16.200.2'
```

先前示例是相同 IP 的标准双向一对一源和目标 NAT。但是，要确保 NAT 流量正确通过隧道，您需要在另一端使用静态路由：

```
set protocols static interface-route 172.16.100.2/32 next-hop-interface 'vfp0'
```

使用静态路由的原因是 IPsec 守护程序已经为远程前缀创建了内核路径：

```
K    *> 172.16.100.0/24 via 169.63.66.49, dp0bond1
```

对源 `10.177.137.251` 执行 ping 操作使其转换为 `172.16.100.2` 时，流量将通过 `dp0bond1` 流出，但无法通过隧道传输，并且绝不会正确匹配 NAT 规则。静态路由解决了此问题：

```
K    *> 172.16.100.0/24 via 169.63.66.49, dp0bond1
S    *> 172.16.100.2/32 [1/0] is directly connected, vfp0
```

这将为流量创建一个更明确的路径来接管 `vfp0`。 

此时，NAT 将按配置工作，并且流量将穿过隧道。 

**注：**使用 NAT 时，您需要指向 `vfp0` 虚拟接口上流量的路径具有的 CIDR 小于 IPsec 远程前缀（大小不能相同）。

一切就绪后，可以对其执行 ping 操作并进行验证：

```
[root@acs-jmat-migserver ~]# ping 172.16.100.1
PING 172.16.100.1 (172.16.100.1) 56(84) bytes of data.
64 bytes from 172.16.100.1: icmp_seq=1 ttl=63 time=44.7 ms
64 bytes from 172.16.100.1: icmp_seq=2 ttl=63 time=44.2 ms
64 bytes from 172.16.100.1: icmp_seq=3 ttl=63 time=44.3 ms
^C
--- 172.16.100.1 ping statistics ---
3 packets transmitted, 3 received, 0% packet loss, time 2003ms
rtt min/avg/max/mdev = 44.247/44.431/44.727/0.272 ms
 
vyatta@acs-jmat-migsim01:~$ show nat source translations
Pre-NAT                 Post-NAT                Prot    Timeout
10.177.137.251:7553     172.16.200.2:7553       icmp    48
```
