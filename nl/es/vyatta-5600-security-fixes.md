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

# Parches de software de AT&T Vyatta 5600 vRouter

**A partir de: 2 de noviembre de 2018**

Este documento contiene los parches para las versiones soportadas actualmente de Vyatta Network OS 5600. Con las versiones 5.2 y anteriores, en los nombres de los parches se utiliza un número S. Con las versiones 17.1 y posteriores, los nombres de los parches tienen una letra minúscula, sin incluir “i”, “o”, “l” y “x”.

Cuando se tratan varios números de CVE en una única actualización, se muestra la puntuación más alta de CVSS.

## 1801t

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-44172 | Bloqueador | Se muestra el error “interfaces [openvpn] no válido” en pruebas mss-clamp |
| VRVDR-43969 | Leve | La GUI de Vyatta 18.x muestra un uso de memoria de comprobación de estado incorrecto |
| VRVDR-43847  | Grave | Rendimiento lento para conversaciones TCP sobre la interfaz de enlace |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR-43842 | N/D | DSA-4305-1 | CVE-2018-16151, CVE-2018-16152: Debian DSA4305-1: strongswan – actualización de seguridad |

## 1801s

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-44041 | Grave | Tiempo de respuesta lento de SNMP ifDescr oid |
 
**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR-44074| 9.1 | DSA-4322-1 | CVE-2018-10933: Debian DSA-4322-1: libssh – actualización de seguridad|
| VRVDR-44054 | 8.8 | DSA-4319-1 | CVE-2018-10873: Debian DSA-4319-1: spice – actualización de seguridad |
| VRVDR-44038 | N/D | DSA-4315-1 | CVE-2018-16056, CVE-2018-16057, CVE-2018- 16058: Debian DSA-4315-1: wireshark – actualización de seguridad |
| VRVDR-44033 | N/D | DSA-4314-1 | CVE-2018-18065: Debian DSA-4314-1: net-snmp – actualización de seguridad | 
|VRVDR-43922 | 7.8 | DSA-4308-1 | CVE-2018-6554, CVE-2018-6555, CVE-2018-7755, CVE-2018-9363, CVE-2018-9516, CVE-2018-10902, CVE-2018-10938, CVE-2018-13099, CVE-2018- 14609, CVE-2018-14617, CVE-2018-14633, CVE- 2018-14678, CVE-2018-14734, CVE-2018-15572, CVE-2018-15594, CVE-2018-16276, CVE-2018- 16658, CVE-2018-17182: Debian DSA-4308-1: linux – actualización de seguridad |
| VRVDR-43908 | 9.8 | DSA-4307-1 | CVE-2017-1000158, CVE-2018-1060, CVE-2018- 1061, CVE-2018-14647: Debian DSA-4307-1: python3.5 - actualización de seguridad |
| VRVDR-43884 | 7.5 | DSA-4306-1 | CVE-2018-1000802, CVE-2018-1060, CVE-2018- 1061, CVE-2018-14647: Debian DSA-4306-1: python2.7 - actualización de seguridad |

## 1801r

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-43738 | Grave | Los paquetes inalcanzables de ICMP devueltos a través de la sesión SNAT no se entregan |
| VRVDR-43538 | Grave | Se reciben errores de exceso de tamaño en interfaz de enlace | 
| VRVDR-43519 | Grave | Vyatta-keepalived se ejecuta sin configuración | 
| VRVDR-43517 | Grave | El tráfico falla cuando el punto final de IPsec basado en VFP/Policy reside en el propio vRouter | 
| VRVDR-43477 | Grave | La confirmación de la configuración de VPN de IPsec devuelve el aviso “Aviso: no se ha podido [VPN toggle net.ipv4.conf.intf.disable_policy], se ha recibido el código de error 65280 |
| VRVDR-43379 | Leve | Las estadísticas de NAT no se muestran correctamente |
 
**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR-43837 | 7.5 | DSA-4300-1 | CVE-2018-10860: Debian DSA-4300-1: libarchive-zip-perl –actualización de seguridad |
| VRVDR-43693 | N/D | DSA-4291-1 | CVE-2018-16741: Debian DSA-4291-1: mgetty –actualización de seguridad | 
| VRVDR-43578 | N/D | DSA-4286-1 | CVE-2018-14618: Debian DSA-4286-1: curl -actualización de seguridad |
| VRVDR-43326 | N/D | DSA-4280-1 | CVE-2018-15473: Debian DSA-4280-1: openssh -actualización de seguridad | 
| VRVDR-43198 | N/D | DSA-4272-1 | CVE-2018-5391: Debian DSA-4272-1: actualización de seguridad de linux (FragmentSmack) |
| VRVDR-43110 | N/D | DSA-4265-1 | Debian DSA-4265-1 : xml-security-c -actualización de seguridad | 
| VRVDR-43057 | N/D | DSA-4260-1 | CVE-2018-14679, CVE-2018-14680, CVE-2018-14681, CVE-2018-14682: Debian DSA-4260-1 : libmspack -actualización de seguridad | 
| VRVDR-43026 | 9.8 | DSA-4259-1 | Debian DSA-4259-1 : ruby2.3 -security updateVRVDR-42994N/ADSA-4257-1CVE-2018-10906: Debian DSA-4257-1 :fuse -actualización de seguridad |

## 1801q

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-43531 | Grave |Un arranque en 1801p colapsa el kernel en unos 40 segundos |
| VRVDR-43104 | Crítico | Falso ARP innecesario sobre red DHCP cuando IPsec está habilitado |
| VRVDR-41531 | Grave | IPsec continúa intentando utilizar la interfaz de VFP después de desenlazarla |
| VRVDR-43157 | Leve | Cuando el túnel salta, la condición de excepción SNMP no se genera correctamente. |
| VRVDR-43114 | Crítico | Tras el rearranque, un direccionador en un par HA con una prioridad superior a la de su igual no respeta su propia configuración "preempt false" y se convierte en el maestro inmediatamente después del arranque |
| VRVDR-42826 | Leve | Con el id remoto “0.0.0.0”, la negociación de iguales falla por discrepancia de pre-shared-key |
| VRVDR-42774 | Crítico| El controlador X710 (i40e) envía tramas de control de flujo a una tasa muy alta |
| VRVDR-42635 | Leve | El cambio de política route-map de redistribución de BGP no tiene efecto |
| VRVDR-42620 | Leve | Vyatta-ike-sa-daemon genera el error “Command failed: establishing CHILD_SA passthrough-peer” cuando parece que el túnel está activo |
| VRVDR-42483 | Leve | Error de autenticación de TACACS |
| VRVDR-42283 | Grave | El estado de VRRP pasa a FAULT para todas las interfaces cuando se suprime la ip de la interfaz vip |
| VRVDR-42244 | Leve | La supervisión de flujo solo exporta 1000 muestras al recopilador |
| VRVDR-42114 | Crítico | El servicio HTTPS NO DEBE exponer TLSv1 |
| VRVDR-41829 | Grave | Volcado de núcleo de plano de datos hasta que el sistema deja de responder con SIP ALG soak test |
| VRVR-41683 | Bloqueador | La dirección de servidor de nombres DNS obtenida sobre VRF no se reconoce correctamente |
| VRVDR-41628 | Leve | Ruta/prefijo desde direccionador-anuncio activo en kernel y en plano de datos, pero ignorado por RIB |
 
**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR-43288 | 5.6 | DSA-4279-1 | CVE-2018-3620, CVE-2018-3646: Debian DSA-4279- 1 – actualización de seguridad de Linux |
| VRVDR-43111 | N/D | DSA-4266-1 | CVE-2018-5390, CVE-2018-13405: Debian DSA- 4266-1 – actualización de seguridad de Linux |

## 1801n

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-42588 | Leve | Configuración de protocolo de direccionamiento confidencial se cuela en registro del sistema |
| VRVDR-42566 | Crítico | Después de actualizar de 17.2.0h a 1801m, un día después se produjeron varios reinicios en ambos miembros de HA |
| VRVDR-42490 | Grave | Error de VTI-IPSEC IKE SA un minuto después de la transición de VRRP |
| VRVDR-42335 | Grave | IPSEC: comportamiento de remote-id “hostname” cambia de 5400 a 5600 |
| VRVDR-42264 | Crítico | Sin conectividad a través del túnel SIT - "kernel: sit: non-ECT from 0.0.0.0 with TOS=0xd" |
| VRVDR-41957 | Leve | Los paquetes NAT bidireccionales son demasiado grandes para GRE; no pueden devolver el código 4 de ICMP Tipo 3 |
| VRVDR-40283 | Grave | Los cambios de configuración generan un montón de mensajes de registro |
| VRVDR-39773 | Grave | Si se utiliza route-map con el mandato de BGP vrrp-failover, se eliminan todos los prefijos |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR-42505 | N/D | DSA-4236-1 | CVE-2018-12891, CVE-2018-12892, CVE-2018-12893: Debian DSA-4236-1: xen - actualización de seguridad |
| VRVDR-42427 | N/D | DSA-4232-1 | CVE-2018-3665: Debian DSA 4232-1: xen - actualización de seguridad |
| VRVDR-42383 | N/D | DSA-4231-1 | CVE-2018-0495: Debian DSA-4231-1: libgcrypt20 - actualización de seguridad |
| VRVDR-42088 | 5.5 | DSA-4210-1 | CVE-2018-3639: Debian DSA-4210-1: xen – actualización de seguridad |
| VRVDR-41924 | 8.8 | DSA-4201-1 | CVE-2018-8897, CVE-2018-10471, CVE-2018-10472, CVE-2018-10981, CVE-2018-10982: Debian DSA-4201- 1: xen – actualización de seguridad |

## 5.2R6S12

Publicado el 21 de junio de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-42084 | Bloqueador | La interfaz de Vfp se marca como "interfaz no de plano de datos" en "show dataplane route" cuando se vuelve a aplicar la configuración nat/ipsec |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR-42317 | 5.4 | DSA-4226-1 | CVE-2018-12015: Debian DSA-4226-1: perl – actualización de seguridad |
| VRVDR-42284 | 7.5 | DSA-4222-1 | CVE-2018-12020: Debian DSA-4222-1: gnupg2 – actualización de seguridad |
| VRVDR-41797 | 8 | DSA-4196-1 | CVE-2018-1087, CVE-2018-8897: Debian DSA-4196-1: linux – actualización de seguridad |
| VRVDR-41680 | 7.8 | DSA-4188-1 | Debian DSA-4188-1: linux – actualización de seguridad (Spectre) |

## 1801m

Publicado el 15 de junio de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-42256 | Crítico | No hay tráfico de salida si se suprime el último CHILD_SA establecido |
| VRVDR-42084 | Bloqueador | Las sesiones NAT enlazadas a las interfaces de VFP para túneles IPsec PB no se crean para los paquetes que llegan al direccionador, aunque el direccionador esté configurado para ello |
| VRVDR-42018 | Leve | Cuando se ejecuta "restart vpn", se genera un error "IKE SA daemon: org.freedesktop.DBus.Error.Service.Unknown". |
| VRVDR-42017 | Leve | Cuando se ejecuta “show vpn ipsec sa” en la copia de seguridad de VRRP, se genera el error “ConnectionRefusedError” relacionado con vyatta-op-vpn- ipsec-vici línea 563 |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 42317 | 5.4 | DSA-4226-1 | CVE-2018-12015: Debian DSA-4226-1: perl – actualización de seguridad |
| VRVDR- 42284 | 7.5 | DSA-4222-1 | CVE-2018-12020: Debian DSA-4222-1: gnupg2 – actualización de seguridad |

## 5.2R6S11

Publicado el 11 de junio de 2018

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-42109 | Crítico | Solo se recibe 1 paquete de respuesta ICMP con SNAT+FW en 5.2R6S7 |
| VRVDR-42084 | Bloqueador | Las sesiones NAT enlazadas a las interfaces de VFP para túneles IPsec PB no se crean para los paquetes que llegan al direccionador, aunque el direccionador esté configurado para ello |
| VRVDR-42027 | Grave | SFLOW utiliza ifIndex de entrada incorrecto |
| VRVDR-41558 | Grave | Las indicaciones de fecha y hora notificadas en los rastreos de paquetes no son coherentes con el tiempo real y el reloj del sistema |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 42207 | 7.5 | DSA-4217-1 | CVE-2018-11358, CVE-2018-11360, CVE-2018-11362, CVE- 2018-7320, CVE-2018-7334, CVE-2018-7335, CVE-2018- 7419, CVE-2018-9261, CVE-2018-9264, CVE-2018-9273: Debian DSA-4217-1: wireshark – actualización de seguridad |
| VRVDR- 42013 | N/D | DSA-4210-1 | CVE-2018-3639: ejecución especulativa, variante 4: omisión almacén especulativa / Spectre v4 / Spectre-NG |
| VRVDR- 42006 | 9.8 | DSA-4208-1 | CVE-2018-1122, CVE-2018-1123, CVE-2018-1124, CVE-2018- 1125, CVE-2018-1126: Debian DSA-4208-1: procps – actualización de seguridad |
| VRVDR- 41946 | N/D | DSA-4202-1 | CVE-2018-1000301: Debian DSA-4202-1: curl – actualización de seguridad |
| VRVDR- 41795 | 6.5 | DSA-4195-1 | CVE-2018-0494: Debian DSA-4195-1: wget – actualización de seguridad |

## 1801k

Publicado el 8 de junio de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-42084 | Bloqueador | Las sesiones NAT enlazadas a las interfaces de VFP para túneles IPsec PB no se crean para los paquetes que llegan al direccionador, aunque el direccionador esté configurado para ello |
| VRVDR-41944 | Grave | Después de la migración tras error de VRRP, algunos túneles de VTI no se restablecen hasta que se emite "vpn restart" o un restablecimiento de igual |
| VRVDR-41906 | Grave | El descubrimiento de PMTU falla porque los mensajes ICMP de tipo 3 y 4 se envían desde de la IP de origen incorrecta |
| VRVDR-41558 | Grave | Las indicaciones de fecha y hora notificadas en los rastreos de paquetes no son coherentes con el tiempo real y el reloj del sistema |
| VRVDR-41469 | Grave | Una interfaz de enlace descendente no carga el tráfico |
| VRVDR-41420 | Grave | Estado de enlace de LACP "u/D" con cambio de modalidad activa-copia de seguridad en LACP |
| VRVDR-41313 | Crítico | IPsec – inestabilidad de la interfaz VTI |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 42207 | 7.5 | DSA-4217-1 | CVE-2018-11358, CVE-2018-11360, CVE-2018-11362, CVE- 2018-7320, CVE-2018-7334, CVE-2018-7335, CVE02018- 7419, CVE-2018-9261, CVE-2018-9264, CVE-2018-9273: Debian DSA-4217-1: wireshark – actualización de seguridad |
| VRVDR- 42013 | N/D | DSA-4210-1 | CVE-2018-3639: ejecución especulativa, variante 4: omisión almacén especulativa / Spectre v4 / Spectre-NG |
| VRVDR- 42006 | 9.8 | DSA-4208-1 | CVE-2018-1122, CVE-2018-1123, CVE-2018-1124, CVE-2018- 1125, CVE-2018-1126: Debian DSA-4208-1: procps – actualización de seguridad |
| VRVDR- 41946 | N/D | DSA-4202-1 | CVE-2018-1000301: Debian DSA-4202-1: curl – actualización de seguridad |
| VRVDR- 41795 | 6.5 | DSA-4195-1 | CVE-2018-0494: Debian DSA-4195-1: wget – actualización de seguridad |

## 1801j

Publicado el 18 de mayo de 2018

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-41481 | Leve | VRRP en interfaz de enlace no envía anuncio de VRRP |
| VRVDR-39863 | Grave | VRRP falla cuando el cliente elimina la instancia de direccionamiento con GRE asociado y el túnel local-dirección forma parte de VRRP |
| VRVDR-27018 | Crítico | El archivo de configuración en ejecución es legible a nivel global |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR-41680 | 7.8 | DSA-4188-1 | Debian DSA-4188-1: linux – actualización de seguridad |

## 5.2R6S10

Publicado el 17 de mayo de 2018

**Problemas resueltos**
| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-41543 | Grave | “update config-sync” genera errores cuando se utiliza la barra inclinada invertida “\” en descripciones de configuración
| VRVDR-27018 | Crítico | El archivo de configuración en ejecución es legible a nivel global |

## 1801h

Publicado el 11 de mayo de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-41664 | Crítico | El plano de datos descarta los paquetes ESP de tamaño MTU |
| VRVDR-41536 | Leve | Se alcanza el límite start-init del servicio Dnsmasq cuando se añaden más de 4 entradas de host estáticas si el reenvío de dns está habilitado |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 41797 | 7.8 | DSA-4196-1 | CVE-2018-1087, CVE-2018-8897: Debian DSA-4196-1: actualización de seguridad de linux |

## 5.2R6S

Publicado el 8 de mayo de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-40803 | Leve | Interfaces VIF no están presentes en la salida de “show vrrp” después de reiniciar |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 41512 | 9.8 | DSA-4172-1 | CVE-2018-6797, CVE-2018-6798, CVE-2018-6913: Debian DSA-4172-1: perl – actualización de seguridad |

## 1801g

Publicado el 4 de mayo de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-41620 | Grave | El tráfico de la interfaz de vTI deja de enviar tráfico después de que se añada vIF nuevo |
| VRVDR-40965 | Grave | El enlace no se recupera después de un bloqueo de un plano de datos |

## 1801f

Publicado el 23 de abril de 2018

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-41537 | Leve | Ping no funciona sobre el túnel IPsec en 1801d |
| VRVDR-41283 | Leve | Configd deja de procesar rutas estáticas durante el arranque si la configuración ha inhabilitado las rutas estáticas |
| VRVDR-41266 | Grave | La ruta estática que se filtra a VRF no transmite el tráfico a través del túnel mGRE después de un rearranque |
| VRVDR-41255 | Grave | Cuando el esclavo se desactiva, el estado de enlace del maestro tarda más de 60 segundos en reflejarlo |
| VRVDR-41252 | Grave | Con la VTI desenlazada en la política de zonas, la regla de eliminación se omite en función del orden de confirmación de las reglas de zona |
| VRVDR-41221 | Crítico | Actualización de vRouters de 1801b a 1801c a 1801d con una tasa de anomalía del 10 % |
| VRVDR-40967 | Grave | La inhabilitación del reenvío IPv6 impide el direccionamiento de paquetes IPv4 de origen de VTI |
| VRVDR-40858 | Grave | Interfaz VTI que muestra MTU 1428 causa problemas de TCP PMTU |
| VRVDR-40857 | Crítico | El puente Vhost no se activa para la VLAN etiquetada con nombres de interfaz de una longitud determinada |
| VRVDR-40803 | Leve | Interfaces VIF no están presentes en la salida de “show vrrp” después de reiniciar |
| VRVDR-40644 | Grave | IKEv1: las retransmisiones QUICK_MODE no se gestionan correctamente |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 41512 | 9.8 | DSA-4172-1 | CVE-2018-6797, CVE-2018-6798, CVE-2018-6913: Debian DSA-4172-1: perl – actualización de seguridad |
| VRVDR- 41331 | 6.5 | DSA-4158-1 |CVE-2018-0739: Debian DSA-4158-1: openssl1.0 – actualización de seguridad
| VRVDR- 41330 | 6.5 | DSA-4157-1 | CVE-2017-3738, CVE-2018-0739: Debian DSA-4157-1: openssl – actualización de seguridad |
| VRVDR- 41215 | 6.1 |CVE-2018-1059 | CVE-2018-1059 – DPDK vhost fuera de acceso de memoria de host enlazada desde invitados de VM |

##5.2R6S8
Publicado el 16 de abril de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-41283 | Leve |Configd deja de procesar rutas estáticas durante el arranque si la configuración ha inhabilitado las rutas estáticas |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 41330 | 6.5 | DSA-4157-1 | CVE-2017-3738, CVE-2018-0739: Debian DSA-4157-1: openssl – actualización de seguridad

##1801e
Publicado el 28 de marzo de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-39985 | Leve | Los paquetes de TCP DF mayores que MTU de túnel GRE se descartan sin que se haya devuelto ninguna fragmentación de ICMP | 
| VRVDR-41088 | Crítico | ASN ampliado (4 bytes) no se representa internamente como tipo sin firma |
| VRVDR-40988 | Crítico | Vhost no se inicia cuando se utiliza con un determinado número de interfaces |
| VRVDR-40927 | Crítico | DNAT: SDP en SIP 200 OK no se convierte cuando sigue a una respuesta 183 |
| VRVDR-40920 | Grave | Con 127.0.0.1 como listen-address snmpd no se inicia |
| VRVDR-40920 | Crítico | ARP no funciona sobre la interfaz SR-IOV enlazada |
| VRVDR-40294 | Grave | El plano de datos no restaura las colas anteriores después de eliminar el esclavo del grupo de enlace |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 41172 | N/D | DSA-4140-1 | DSA 4140-1: actualización de seguridad de libvorbis |

##5.2R6S7
Publicado el 15 de marzo de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-38801 | Grave | El paquete de varios segmentos recibido a través de IPsec VTI hace que caiga la interfaz de enlace

##5.2R6S6
Publicado el 12 de marzo de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-40281 | Grave | Después de actualizar de 5.2 a una versión más reciente aparece el error "vbash: show: no se encuentra el mandato" en modalidad de operación |
| VRVDR-40135 | Grave | Los paquetes de árbol de expansión no se reciben en un puerto de puente de interfaz VIF |
| VRVDR-39991 | Grave | El cortafuegos con estado descarta paquetes entre dos subredes de la misma interfaz | 
| VRVDR-36481 | Grave | Actualización/degradación de 5.2R4 a 17.1.0/5.2R3 muestra /opt/vyatta/sbin/vyatta-install-image.functions: línea 372: is_onie_boot: no se ha encontrado el mandato |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 40019 | 8.8 | DSA-4086-1 | CVE-2017-15412: Debian DSA-4086-1: libxml2 – actualización de seguridad |
| VRVDR- 39907 | 7.8 | CVE-2017-5717 | Inyección destino rama / CVE-2017-5717 / Spectre, Variante 2 |

##1801d
Publicado el 8 de marzo de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-40940 | Grave | Caída del plano de datos relacionada con NAT/cortafuegos |
| VRVDR-40886 | Grave | La combinación de “icmp name <value>” con un número de otra configuración para la regla hace que no se cargue el cortafuegos |
| VRVDR-39879 | Grave | La configuración de enlaces para tramas jumbo falla |

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 40327 | 9.8 | | DSA-4098-1
CVE-2018-1000005, CVE-20178-1000007: Debian DSA- 4098-1: curl – actualización de seguridad | 
| VRVDR- 39907 | 7.8 | CVE-2017-5717 | Inyección destino rama / CVE-2017-5715 / Spectre, variante 2 |

##1801c
Publicado el 7 de marzo de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-40281 | Grave | Después de actualizar de 5.2 a una versión más reciente aparece el error "-vbash: show: no se encuentra el mandato" en modalidad de operación |

##1801b
Publicado el 21 de febrero de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-40622 | Grave | Las imágenes de cloud-init no pueden detectar correctamente si la dirección IP se ha obtenido del servidor DHCP |
| VRVDR-40613 | Crítico | La interfaz de enlace no se activa si uno de los enlaces físicos está inactivo |
| VRVDR-40328 | Grave | Las imágenes de cloud-init tardan mucho tiempo en arrancar |

##1801a
Publicado el 7 de febrero de 2018.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-40324 | Grave | Los promedios de carga exceden 1.0 sin carga en el direccionador con interfaz de enlace |

##5.2R6S5
Publicado el 19 de enero de 2018.

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 39891 | 5.6 | DSA-4078-1 | CVE-2017-5754: Debian DSA-4078-1: linux – actualización de seguridad (Meltdown) |
| VRVDR- 38265 | 8.8 | DSA-3970-1 | CVE-2017-1 |

##5.2R6S4
Publicado el 15 de diciembre de 2017.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-39529 | Grave | La migración tras error del servidor DHCP no sincroniza las bases de datos |
| VRVDR-39399 | Crítico | Vyatta genera ERROR de estado de red en show vrrp/múltiples interfaces/error de seg/flap |
| VRVDR-39112 | Grave | El tráfico DNAT que coincide con ZBF solo procesa el primer paquete del flujo |
| VRVDR-38075 | Leve | Cuando se emite la respuesta “restart vpn”, el iniciador no restablece la conexión |
| VRVDR-37934 | Crítico | Caída de BGPd cuando aggregate-address summary-only está configurado/faltan rutas estáticas |
| VRVDR-37717 | Leve | Cambio de nombre de los campos “Description” y “License” en salida de versión |
| VRVDR-37689 | Grave | Alta tasa de interrupciones de NIC PF |
| VRVDR-37633 | Crítico | Keepalived se cuelga |

## 5.2R6S3
Publicado el 4 de diciembre de 2017.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-39207 | Crítico | Error de ARP en interfaz VIF de enlace |


##5.2R6S2
Publicado el 2 de Noviembre de 2017.

**Problemas resueltos**

| Número de problema | Prioridad | Resumen |
| --- | --- | --- |
| VRVDR-39177 | Grave | La opción domain-name de servidor OpenVPN no se aplica con la opción -push dhcp |
| VRVDR-39129 | Crítico | El parámetro push-route del servidor OpenVPN provoca que OpenVPN no se inicie |

##5.2R6S1
Publicado el 12 de octubre de 2017.

**Vulnerabilidades de seguridad resueltas**

| Número de problema | Puntuación CVSS | Advertencia | Resumen |
| --- | --- | --- | --- |
| VRVDR- 38819 | 9.8 | DSA-3989-1 | CVE-2017-14491, CVE-2017-14492, CVE-2017-14493, CVE- 2017-14494, CVE-2017-14495, CVE-2017-14496: DSA- 3989-1 dnsmasq -- actualización de seguridad |

La información aquí contenida no es una oferta, compromiso, representación ni garantía por parte de AT&T y está sujeta a cambios. No se debe utilizar ni distribuir fuera de empresas AT&T, excepto bajo acuerdo escrito.

© 2018 AT&T Intellectual Property. Todos los derechos reservados. AT&T y el logotipo de Globe son marcas registradas de AT&T Intellectual Property. Todas las demás marcas son propiedad de sus respectivos propietarios.
