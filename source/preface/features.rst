Leistungsmerkmale
=================

Basisfeatures
-------------

Der Kern von linuxmuster.net 6.1 besitzt folgende Leistungsmerkmale:

-  Komplett **quelloffene** Software
-  Unveränderter Ubuntu Server 12.04 LTS als Grundlage.

   -  **Vollautomatische Installation** benötigter Serverkomponenten.
   -  Aktualisierung der linuxmuster.net Installation über die
      standardmäßige **Debian Paketverwaltung**.
   -  **Rückwärtskompatibel** mit Linux Musterlösungen (paedML,openML)
      über Datenmigration

-  **SheilA-Konzept** (Abkürzung für *Selbstheilende Arbeitsstationen*)
   durch LINBO: Restaurieren von Arbeitsstationen auf Knopfdruck.

   -  Halbautomatische Aufnahme der Arbeitsstationen in den DHCP- und
      DNS-Server.

-  **Firewall-Lösung** durch IPFire - Abschirmung nach außen und
   Sicherheit im internen Netzwerk (Paketfilter, auch für ausgehende
   Verbindungen).
-  Filterung problematischer Internet-Inhalte durch Bereichsfilterung
   (Pornografie, Gewalt, Drogen, Raubkopien, etc.) und URL-Filter mit
   White- und Blacklists basierend auf Squid.
-  Schulkonsole: Weboberfläche zur **Steuerung der Funktionen im
   Unterricht** durch den Lehrer und der Administration durch den
   Netzwerkbetreuer.

   -  Sichere Umgebung für Klassenarbeiten und Abschlussprüfungen am
      Rechner.
   -  Drucker- und Internetzugang raumweise an- und abschaltbar.

-  **Schulspezifische Benutzerverwaltung** des LDAP-Servers über
   sophomorix
-  Remote Administration per SSH oder OpenVPN
-  Arbeiten im pädagogischen Netzwerk durch

   -  zentrale Benutzerverzeichnisse auf dem Server (Windows- und
      Linux-Clients) mit Samba 3 als Fileserver,
   -  Tauschverzeichnisse für verschiedene Gruppen (Schule, Lehrer,
      Klassen, Projekte).

-  **Komplettes Intranet** (Mailserver inkl. Virenscanner, Webserver mit
   CGI-Perl, PHP, Datenbanken) und der vorkonfigurierten Groupware
   **Horde 3**: Verschlüsselter Webzugang (VPN,SSL) auf eigene Daten vom
   Schulnetz und von zu Hause für Schüler und Lehrer und optional Zugang
   zu E-Mail

Optionale unterstützte Erweiterungen
------------------------------------

Fertig vorbereitet und installierbar sind folgende optionale Merkmale:

-  **WLAN-Hotspot Funktion** über einen Portal-Server in abgetrenntem
   Netzwerk mit choovachili und einem Radius-Server
-  Einfache Verwaltung von **Druckerkontingenten** mit Pykota
-  Aktives und proaktives **Monitoring** des Servers mit Nagios.
-  Integration von Opsi, einem **Clientmanagement-System** zur
   Verwaltung von Windows-Clients

Optionale durch die Community bereitgestellte Erweiterungen
------------------------------------------------------------
Von der Community getragene Addons erweitern die Lösung um folgende
Merkmale:

-  Weitere Webapplikationen:

   -  **Schulportfolio** in Wikiformat durch openSchulportfolio/dokuwiki
   -  Digitales Medien- und **Raumbuchungssystem** durch MRBS
   -  Lernplattform **Moodle**

-  Die Backup-Lösung *linuxmuster-backup* inkl. Disasterrecovery mit
   **MondoRescue**,
-  **Konfigurable virtuelle Umgebungen** auf einem Linuxclient mit
   *leoclient*
-  Fertiges, vorkonfiguriertes, Abbild für die sofortige Einrichtung von
   Linuxclients

Viele weitere Funktionen sind über das
`Anwenderwiki <http://www.linuxmuster.net/wiki/anwenderwiki:start>`__
von der Community dokumentiert und über das
`Forum <http://forum.linuxmuster.net/>`__ erhält man direkten Support
von der Community und den Entwicklern. Über die `öffentliche
Mailingliste von
linuxmuster.net <https://mail.lehrerpost.de/mailman/listinfo/linuxmuster-user>`__
erhalten Anfragen in außergewöhnlich kurzen Reaktionszeiten Antworten
durch die Community.
