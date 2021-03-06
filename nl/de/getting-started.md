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


# Einführung
Navigieren Sie für den Einstieg in IBM Virtual Router Appliance (VRA) zur Bestellseite im Kundenportal:

1. Rufen Sie in Ihrem Browser das [Kundenportal ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){: new_window} auf und melden Sie sich bei Ihrem Konto an.
2. Wählen Sie im Navigationsbereich des Kundenportals **Netz > Gateway-Appliances** aus.
3. Klicken Sie auf der Listenseite **Gateway-Appliances** auf **Gateway bestellen**.
4. Wählen Sie auf der Seite **Bestellung** im Dropdown-Menü das gewünschte Rechenzentrum aus und wählen Sie anschließend den gewünschten Typ der Server-Hardware aus.

    **HINWEIS:** Die Server-Mindestanforderungen für VRA sind 8 GB RAM und ein CPU-Kern für jeweils 10 Gb/s Netzkapazität. Beispiel: Für ein System mit jeweils 10 Gb/s für öffentliche und private Uplinks sind mindestens 4 Kerne erforderlich. Reservieren Sie mehr als die Standardeinstellung für den Plattenspeicher, wenn Sie Netzdiagnosen ausführen möchten, die detaillierte Protokolle erstellen. Wenn Sie beabsichtigen, VPN-Services mit Verschlüsselung einzurichten, wollen Sie möglicherweise weitere zentraler Bestandteile hinzufügen. Das Hinzufügen weiterer zentraler Bestandteile für VPN-Services garantiert, dass die VRA nicht durch eine hohe Auslastung und gleichzeitige Ver- bzw. Entschlüsselung von Daten zum Erliegen kommt.

5. Wählen Sie auf der Anforderungsseite bei Bedarf die Option **HA-Paar** aus, wählen Sie in jedem Fall die Hauptspeichergröße und die entsprechende Version des VRA-Betriebssystems und anschließend die Uplinkgeschwindigkeit für das Netz aus. 

6. Überprüfen Sie die von Ihnen getroffenen Auswahlen und klicken Sie anschließend auf **Zur Bestellung hinzufügen**. Die Bestellung wird automatisch geprüft.
7. Wählen Sie auf der Seite **CHECKOUT** (wenn Sie bereits über eigene VLANs in dem ausgewählten Rechenzentrum verfügen) die Back-End-VLANs aus, die geschützt werden müssen. Geben Sie einen Hostnamen und einen Domänennamen für Ihre VRA an. Wählen Sie alle Kontrollkästchen für IBM Cloud-Service-Bedingungen und für Servicevereinbarungen Dritter aus. Klicken Sie anschließend auf **Bestellung absenden**.

Nachdem Ihre Bestellung genehmigt ist, wird die Bereitstellung Ihrer VRA automatisch gestartet. Wenn der Bereitstellungsprozess abgeschlossen ist, wird die neue VRA auf der Listenseite **Gateway-Appliances** angezeigt. Klicken Sie auf den Namen des Gateways, um die Seite **Gateway-Details** zu öffnen und klicken Sie anschließend auf jedes Gateway-Member, um die Seite **Einheitendetails** zu öffnen. Diese Seite enthält die IP-Adressen, sowie den Anmeldebenutzernamen und das Kennwort für das Gerät.  

**HINWEIS:** Es ist wichtig, dass Sie nicht vergessen, das Gerät selbst unbedingt mit denselben Einstellungen zu konfigurieren, sobald Sie Ihre VRA im IBM Cloud Customer Portal bestellt und konfiguriert haben. 

## VLANs und die Rolle der Gateway-Appliance
Ein VLAN (virtuelles LAN) ist ein Mechanismus, der ein physisches Netz in mehrere virtuelle Segmente aufteilt. Aus Gründen des Bedienungskomforts kann der Datenverkehr von mehreren ausgewählten VLANs über ein einzelnes Netzübertragungskabel übermittelt werden (diese Methode wird allgemein als "Trunking" bezeichnet).

VRA wird in zwei Teilkomponenten bereitgestellt: VRA-Server und Gateway-Appliance-Komponente. Die Gateway-Appliance stellt eine Schnittstelle (GUI und API) zum Auswählen der VLANs bereit, die Sie Ihrer VRA zuordnen möchten. Durch das Zuordnen eines VLANs mit einer Gateway-Appliance werden das VLAN und alle zugehörigen Teilnetze zu Ihrer VRA umgeleitet, damit Sie die Filterung, die Weiterleitung und die Schutzmaßnahmen steuern können. Server in einem zugeordneten VLAN sind für andere VLANs nur über Ihre VRA erreichbar und die VRA kann nur umgangen werden, wenn Sie das VLAN übergehen oder die Zuordnung aufheben.

Eine neue Gateway-Appliance wird standardmäßig zwei nicht entfernbaren Durchgangs-VLANs zugeordnet (eines für öffentliche Daten und eines für private Daten). Diese VLANs werden in der Regel für administrative Aufgaben verwendet und können durch VRA-Befehle geschützt werden.

Transit-VLANs sind für Netzeinheiten wie Firewalls oder Lastenverteilerfunktionen konzipiert, um Datenverkehr weiterzuleiten, während andere Geräte oder Einheiten wie Server oder Container vom Internet isoliert bleiben. 

Im Unterschied dazu werden auf 'Gateway'-VLANs Einheiten wie beispielsweise Server und Container gehostet. 

VRA kann nur VLANs, die ihr zugeordnet sind, über die Gateway-Appliance verwalten.

Weitere Informationen zum Verwalten von VLANs in der Anzeige 'Gateway-Appliance-Details' finden Sie im Abschnitt [VLANs verwalten](manage-vlans.html).
