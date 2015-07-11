`migration <http://www.linuxmuster.net/wiki/tag:migration?do=showtag&tag=tag%3Amigration>`__

Migrationspfade im Überblick
============================

Das Paket linuxmuster-migration
-------------------------------

Das Paket
`linuxmuster-migration <https://github.com/linuxmuster/linuxmuster-migration>`__
stellt eine Sammlung von Shellskripten zur Verfügung, die es
ermöglichen, sämtliche System- und Benutzerdaten zwischen
openML/linuxmuster.net-Systemen zu übertragen.

Features
^^^^^^^^

Migration

-  der kompletten IPCop- und Serverkonfiguration inklusive Zertifikate,
   Samba-SID und LINBO-Images.
-  sämtlicher Postgresql- und MySQL-Datenbanken inklusive
   Benutzerkonfiguration.
-  aller Benutzerdaten inklusive Passwörter.
-  zusätzlich aus Fremdquellen installierter Softwarepakete.
-  auf aktuellere Version:

   -  z.Zt. unterstützte Quellsysteme: paedML >= 4.0.6, openML/paedML
      5.x, linuxmuster.net 6.x
   -  z.Zt. unterstützte Zielsysteme: openML/paedML 5.x, linuxmuster.net
      6.0, linuxmuster.net 6.1.

IPCop vs. IPFire
----------------

-  Falls der IPCop dediziert installiert wurde (`Umstellen auf
   dedizierten
   IPCop <http://www.linuxmuster.net/wiki/dokumentation:handbuch51:ipcop:umstellung_dediziert>`__
   im Handbuch der Version 5.1) ist die Migration des Servers problemlos
   unter Beibehaltung der IPCop Konfiguration möglich. In einem weiteren
   Schritt kann der IPCop durch IPFire ersetzt werden (`Umstieg von
   IPCop auf
   IPFire <http://www.linuxmuster.net/wiki/dokumentation:handbuch61:installation:ipcop2ipfire>`__).

-  Die Migration von **openML 4.x/5.x** mit IPCop zu **linuxmuster.net
   6.x** mit IPFire ist ebenfalls problemlos möglich.
   OpenVPN-Zertifikate werden migriert, eigene Firewalleinstellungen
   werden allerdings nicht übernommen. Diese müssen später wieder von
   Hand eingepflegt werden. Die Vorgehensweise unterscheidet sich nicht
   von derjenigen mit IPCop zu IPCop. Man setzt ein Grundsystem mit
   `IPFire <http://www.linuxmuster.net/wiki/dokumentation:handbuch61:installation:ipfire>`__
   und
   `linuxmuster.net-Server <http://www.linuxmuster.net/wiki/dokumentation:handbuch61:installation:server>`__
   auf und spielt dann nach Anleitung die Daten zurück.

REMBO vs. LINBO
---------------

-  Um von openML 4.0.6 mit REMBO als Imagingsystem auf Linuxmuster
   Version 6.x migrieren zu können, muss man den Server auf LINBO
   umstellen. Siehe dazu im Handbuch zur Version 5.1 `Umstellung auf den
   Betrieb mit
   LINBO <http://www.linuxmuster.net/wiki/dokumentation:handbuch51:clients:linbo:umstellung>`__

Bekannte Probleme
-----------------

Wenn im Zuge der Migration das Serverzertifikat erneuert wurde, muss
jeder Nutzer beim ersten Aufruf einer Schulwebseite (Schulkonsole,
Horde, Moodle etc.) per https das Serverzertifikat erneut akzeptieren.
Das gilt ebenso, wenn ein E-Mail-Client (z.B. Thunderbird) benutzt wird.

-  Bitte prüfen, ob die Dateisystemreihenfolge für die Festplattenquota
   noch stimmt.
-  `Anmeldeproblem mit Ubuntu-12.04-Client nach Migration auf
   linuxmuster.net 6 <http://www.linuxmuster.net/trac/ticket/107>`__
   (Gelöst)
-  `Cyrus-Datenbankfehler nach Migration auf linuxmuster.net
   6 <http://www.linuxmuster.net/trac/ticket/108>`__ (Gelöst)
-  `Nagios-Mailflut nach Migration auf linuxmuster.net
   6 <http://www.linuxmuster.net/trac/ticket/109>`__ (Gelöst)

Handbuch linuxmuster.net 6.1
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

|Zurück...|\ `Zurück... <http://www.linuxmuster.net/wiki/dokumentation:handbuch61:installation:ipfire.defaultconfig>`__

|Inhaltsverzeichnis|\ `Inhaltsverzeichnis <http://www.linuxmuster.net/wiki/dokumentation:handbuch61:start>`__

des Handbuchs

|Weiter...|\ `Weiter... <http://www.linuxmuster.net/wiki/dokumentation:handbuch61:installation:migration.stepbystep>`__

.. |Zurück...| image:: dokumentation:handbuch61:installation:migration.overview-Dateien/dokumentationhandbuchiconsdoc-go-previous.png
   :target: http://www.linuxmuster.net/wiki/dokumentation:handbuch61:installation:ipfire.defaultconfig
.. |Inhaltsverzeichnis| image:: dokumentation:handbuch61:installation:migration.overview-Dateien/dokumentationhandbuchiconsdoc-go-home.png
   :target: http://www.linuxmuster.net/wiki/dokumentation:handbuch61:start
.. |Weiter...| image:: dokumentation:handbuch61:installation:migration.overview-Dateien/dokumentationhandbuchiconsdoc-go-next.png
   :target: http://www.linuxmuster.net/wiki/dokumentation:handbuch61:installation:migration.stepbystep
