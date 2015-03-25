Metainformationen zum Installationshandbuch
-------------------------------------------

Das Installationshandbuch wird aus den reStructuredText-Dateien (*.rst)
mit dem pyhton-Programm sphinx erzeugt. Nähere Inforamtionen erhält man 
hier: http://sphinx-doc.org/index.html

Auf einem debian-basierdenen Linux System kann sphinx einfach 
durch 

    sudo apt-get install python3-sphinx

installiert werden.

Dokumentation erzeugen
----------------------

### HTML-Ausgabe


Wenn man sich im Stammverzeichnis des Repositories befinden, kann man (bei installiertem make) mit dem Befehl

    make html 

die HTML-Version des Handbuchs im Verzeichnis `build/html` erzeugen.

### PDF-Ausgabe

Wenn auf dem System eine funktionsfähige pdflatex-Installation vorhanden ist, kann man mit dem Befehl

    make latexpdf

eine PDF Version des Handbuchs erzeugen. Diese wird im Verzeichnis `build/latex` erstellt.



