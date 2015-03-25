
Hardwareanforderungen
=====================

Die für den Betrieb von linuxmuster.net benötigte Serverhardware hängt stark vom 
konkreten Einsatzszenario ab:

- Werden alle für den Betrieb nötigen linuxmuster.net Server als virtuelle Maschinen auf einem Virtualisierungshost betrieben (empfohlen) oder werden die Maschinen auf dedizierter Hardware installiert?
- Wie groß ist die zu versorgende Infrastruktur? linuxmuster.net kommt sowohl an Grundschulen mit 50 Schülern, 6 Lehrern und 15 Clientrechner zum Einsatz als auch in großen Berufsschulen mit 3000 Schülern, 180 Lehrern und 600 Clientrechnern. Es versteht sich von selbst, dass die serverseitig eingesetzte Hardware sich hier stark unterscheidet.    

Im folgenden sollen exemplarisch einige Eckdaten für verschiedene "Standardszenarien" angegeben werden, mit Hilfe derer sich abschätzen lässt, welche Anforderungen die Hardware für ein geplantes Netz erfüllen sollte. 

Die kleine Lösung
------------------
Im Szenario der "kleinen Lösung" gehen wir von einer kleinen Schule  aus:

- 10-20 Lehrer
- 50-250 Schüler
- Ein Computerraum mit 20 Clients
- Möglicherweise einige mobile Geräte wie iPads, die per WLan einen Zugang zum Internet erhalten sollen

Ein Server mit den folgenden Eckdaten sollten für einen störungfreien, virtualisierten Betrieb von linuxmuster.net ausreichen:

- Aktuelle 4-Kern Server CPU 
- 16GB RAM
- 2 x 1TB Festplatte im Software-Raid 0 (kein Hardware-Raid-Controller nötig)
- 4 x Gbit Netzwerkschnittstelle Kupfer (es ist auch möglich, mit weniger Schnittstellen auszukommen, wenn VLans zum Einsatz kommen) 

Auf dem Server werden je nach Szenario 2-3 virtuelle Maschinen installiert: 

- linuxmuster.net Server
- linuxmuster.net Firewall (IPFire)
- Wenn ein WLan eingesetzt werden soll eventuell ein HotSpot-Server (Chillispot)


