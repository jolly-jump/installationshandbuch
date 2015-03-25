Versionsgeschichte und Changelog
================================

Releaseinformationen zur Version 6.1
------------------------------------

-  Bereitstellung **vorgefertigter virtueller Maschinen** zur einfachen
   Installation in virtuelle Umgebungen
-  Umstellung der internen und externen Firewall auf **IP-Basis**
-  **Subnetting und VLANs** erlauben eine saubere Segmentierung größerer
   Netzwerke und logische Trennung von Lehrer- und Pädagogischem
   Netzwerk im Einklang mit aktuellen datenschutzrechtlichen
   Bestimmungen
-  Neuerungen ab **Linbo 2.2.x**:

   -  Effiziente Zusammenarbeit mit Opsi
   -  Reaktivierung von individuellen Windows 7-Clients
   -  Verbesserter Umgang mit WLAN-Clients
   -  Verkleinerung von LINBO (und damit schnellerer Bootvorgang) durch
      effizientere Komprimierung
   -  Vereinfachte und erweiterte Konfiguration beim PXE-Boot

-  Geänderte Struktur der **Tauschverzeichnisse**: Tausch-, Vorlagen-
   und Schülerverzeichnisse einheitlicher erreichbar
-  **Integration von Opsi**, einem Clientmanagement-System zur
   Verwaltung von Windows-Clients
-  Bereitstellung **vorgefertiger Linuxclients**

-  Unterstützung von Windows XP als Client wird mit dem offiziellen
   Support-Ende von Microsoft eingestellt
-  linuxmuster-backup inkl. Disasterrecovery mit Mondo wird fortan von
   der Community bereitgestellt. Das Migrationsskript übernimmt die
   Funktion des Backups und Restores der Server- und
   Firewallkonfiguration
-  Die Funktion des „remoteadmin“ wird mangels Nutzung entfernt

Details findet man in der
`Veröffentlichungsmitteilung <http://www.linuxmuster.net/wiki/dokumentation:techsheets:release61>`__

Releaseinformationen für frühere Versionen
------------------------------------------

Releaseinformationen zur Version 6.0
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. code:: code

    cat /etc/issue
    linuxmuster.net 6.0.46 / Codename ObenBleiben

Veröffentlichungsdatum: März 2013

-  Ubuntu 12.04 LTS 64bit als Server-Betriebssystem mit Support durch
   Sicherheitsupdates von `Canonical <http://www.canonical.com/>`__ bis
   April 2017.
-  **Sämtliche System- und Nutzerdaten** können einfach von einem
   openML/paedML-System ab Version 4.0.6 übernommen werden.
-  Mit **Linbo 2.1** werden einige Bugs gefixt und die Partitionierung
   von SSDs optimiert. Eine Neupartitionierung und Neuerstellung eines
   Images einer Hardwareklasse kann nötig sein, siehe `LINBO 2.1:
   Besseres
   Partitionieren <http://www.linuxmuster.net/wiki/linuxmusternet:blog:articles:20121113_linbo_verbessertes_partitionierungsverhalten>`__.
-  `IPFire <http://www.ipfire.org/>`__ ist nun die **Standardfirewall**,
   siehe `IPFire: Ein weiterer Schritt
   voran <http://www.linuxmuster.net/wiki/linuxmusternet:blog:articles:20130128_ipfire_ein_weiterer_schritt_voran>`__.
   Zertifikate können von IPCop übernommen werden, der Umstieg wird
   empfohlen.
-  Die Dokumentation zieht um in das
   `Wiki <http://www.linuxmuster.net/wiki/dokumentation:handbuch:start>`__
   und entsteht als Community-Leistung auf Basis der Dokumentation der
   bisherigen PaedMLs/openMLs.
-  Die Schulkonsole bekommt ein moderneres verbessertes Layout.
-  Standard-Linuxclient ist ein von der Community bereitgestelltes
   vorkonfiguriertes Ubuntu 12.04 LTS Abbild, das heruntergeladen werden
   darf. Ebenfalls wird ein virtualisiertes Windows durch die `Leoclient
   Pakete <http://www.linuxmuster.net/wiki/entwicklung:linuxclient:leoclient>`__
   möglich.

-  Das Paket ``sophomorix-virusscan`` durchsucht konfigurierbar die
   Daten nach Viren mit „clamav“.
-  Der Workstation-Import wurde beschleunigt.
-  Italc kann für Linux-Clients besonders komfortabel konfiguriert
   werden.
-  Samba: Sogenannte „bind mounts“ erlauben reibungslosen gemischten
   (Windows+Linux) Client Betrieb.
-  Die Syntax einiger Konfigurationsdateien wurden in manpages
   dokumentiert (``man schueler.txt``)
-  Umzug des Quellcodes nach
   `https://github.com/linuxmuster <https://github.com/linuxmuster>`__
-  Moodle ist nicht mehr standardmäßig installiert, wird von der
   `Community <http://www.linuxmuster.net/wiki/anwenderwiki:webapps:moodle:start>`__
   weitergeführt und unterstützt.
-  Rembo wird nicht mehr unterstützt, es kann zu LINBO umgestellt
   werden.

Details findet man `in der
Veröffentlichungsmitteilung <http://www.linuxmuster.net/wiki/linuxmusternet:blog:articles:20130304_linuxmuster.net_6.0_veroeffentlicht>`__.

Releaseinformationen zur Version 5.1.0
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

-  LINBO 2(Einen kurzen Überblick über einige Neuerungen bietet
   `http://lml.support-netz.de/trac/wiki/LINBO-2.0-Neu <http://lml.support-netz.de/trac/wiki/LINBO-2.0-Neu>`__.):

   -  Verbesserte Client-Gui.
   -  Erweiterte Autostartfunktion.
   -  Vereinfachte Domänenaufnahme für Windowsclients(Siehe dazu
      `http://lml.support-netz.de/trac/blog/Domaenenbeitritt\_vereinfacht <http://lml.support-netz.de/trac/blog/Domaenenbeitritt_vereinfacht>`__.).
   -  Verbessertes Syncverhalten bei NTFS-Partitionen.
   -  Erweiterte HW-Unterstützung durch aktuellen Kernel 3.2.6.
   -  Neue Raum-Option für linbo-remote(Siehe Abschnitt `Fernsteuerung
      per
      SSH <http://www.linuxmuster.net/wiki/dokumentation:handbuch51:clients:linbo:linbo_remote>`__.).

-  Installation von USB-Stick(Vorgehensweise siehe
   `http://lml.support-netz.de/trac/wiki/USB-Installation <http://lml.support-netz.de/trac/wiki/USB-Installation>`__).
-  Bessere Unterstützung aktuellerer Serverhardware durch Umstellung auf
   Kernel 2.6.32-35~bpo50+1.
-  Skripte zur Datenmigration(Siehe dazu
   `http://lml.support-netz.de/trac/wiki/Datenmigration <http://lml.support-netz.de/trac/wiki/Datenmigration>`__).
-  Zahlreiche Fehlerkorrekturen(Einen detailierten Überblick über alle
   Bugfixes und sonstigen Änderungen seit Version 5.0.4 erhalten Sie
   unter
   `support-netz.de <http://lml.support-netz.de/trac/query?status=closed&group=resolution&milestone=5.1.0>`__).
-  Wegfall der Installationsvarianten Integrierter IPCop und
   Rembo-Imaging.
-  Bekannte Fehler:

   -  Installation mit Rootpartition auf Software-Raid schlägt
      fehl(Siehe dazu
      `http://lml.support-netz.de/trac/ticket/585 <http://lml.support-netz.de/trac/ticket/585>`__).
   -  Backup auf Systemen mit Kernel 2.6.32 bleibt hängen(Siehe dazu
      `http://lml.support-netz.de/trac/ticket/595 <http://lml.support-netz.de/trac/ticket/595>`__).

