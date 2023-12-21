# MAGELLAN Datenstruktur

Dies ist der Quellcode zur Datenstruktur-Dokumentation von [MAGELLAN](https://magellan.stueber.de). Die Dokumentation ist Open Source und wir haben sie mit [SQLDocs](https://github.com/openpotato/sqldocs) und [MkDocs](https://www.mkdocs.org/) realisiert.

## SQLDocs unter Windows installieren

1. Lade Dir die die aktuellste Version der [.NET 8 Runtime](https://dotnet.microsoft.com/en-us/download/dotnet/8.0) für Windows herunter.

2. Starte das Installationspaket und beantworte alle Fragen.

3. Gehe auf die [SQLDocs-Download-Seite](https://github.com/openpotato/sqldocs/releases/latest) und lade Dir die aktuellste Version für Windows herunter. 

4. Starte das Installationspaket und beantworte alle Fragen.

## MkDocs unter Windows installieren

1. Installiere [Python](https://www.python.org). Gehe dazu auf die [Python-Download-Seite](https://www.python.org/downloads/) und lade Dir die aktuellste Version für Windows herunter. 

2. Starte das Installationspaket und beantworte alle Fragen.

3. Öffne die Eingabeaufforderung als Administrator.

4. Tippe die Befehle `python --version` und `pip --version` ein, um die Python-Installation zu überprüfen. In beiden Fällen sollte eine Versionsnummer als Ausgabe in der Eingabeaufforderung erscheinen.

5. Tippe jetzt den Befehl `pip install mkdocs mkdocs-material mkdocs-awesome-pages-plugin mkdocs-minify-plugin`, um das Python-Packages MkDocs, das Theme [Material for MkDocs](https://squidfunk.github.io/mkdocs-material), das MkDocs-Plugin [MkDocs Awesome Pages](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin) und das MkDocs-Plugin [mkdocs-minify](https://github.com/byrnereese/mkdocs-minify-plugin) zu installieren.

6. Ein letzter Test: Tippe den Befehl `mkdocs --version` ein. Eine Versionsnummer in der Eingabeaufforderung zeigt Dir erneut, dass alles korrekt installiert wurde.

## Repository klonen

Dieses Repository ist ein Git-Repository. Um das Repository auf deinem lokalen Computer zu klonen, benötigst Du einen Git-Client. Entweder Du installierst Dir [Git für Windows](https://gitforwindows.org/) und arbeitest mit der Eingabeaufforderung, oder Du installierst Dir eine der zahlreichen GUIs. Zu empfehlen wären [GitHub Desktop](https://desktop.github.com) oder [SourceTree](https://www.sourcetreeapp.com).

1. Erstelle einen lokalen Ordner für die Dokumentation, z.B. `c:\docs\sql.magellan.de`.

2. Starte die Eingabeaufforderung und wechsle in den Ordner `c:\docs\sql.magellan.de`.

3. Tippe den Befehl `git clone https://github.com/stuebersystems/sql.magellan.de.git` ein, um das Repository zu klonen.

## Mit SQLDocs arbeiten

Die Rohinformationen zur Datenstruktur findest Du in folgenden Dateien:

+ `c:\docs\sql.magellan.de\v11\dbschema.json`: Datenstruktur für MAGELLAN 11.
+ `c:\docs\sql.magellan.de\v10\dbschema.json`: Datenstruktur für MAGELLAN 10.
+ `c:\docs\sql.magellan.de\v9\dbschema.json`: Datenstruktur für MAGELLAN 9.
+ `c:\docs\sql.magellan.de\v8\dbschema.json`: Datenstruktur für MAGELLAN 8.
+ `c:\docs\sql.magellan.de\v7\dbschema.json`: Datenstruktur für MAGELLAN 7.

Jede Änderung an einer dieser vier Dateien muss mit SQLDocs in das jeweilige MkDocs-Projekt übertragen werden.

Im folgenden die Vorgehensweise für MAGELLAN 11:

1. Starte die Eingabeaufforderung und wechsle in den Ordner `c:\docs\sql.magellan.de\v11`.

2. Tippe den Befehl `sqldocs build-mkdocs -l de -db firebird -s dbschema.json -o .` ein. Das MkDocs-Projekt wird aktualisiert.

Anschließend kannst Du mit MkDocs die Dokumentation neu generieren.

## Mit MkDocs arbeiten

Du hast Python und MkDocs installiert und Du hast dieses Repository geklont oder als Zip-Archiv heruntergeladen. Jetzt kannst Du die Dokumentation lokal auf deinem Rechner generieren:

Im folgenden die Vorgehensweise für MAGELLAN 11:

1. Starte die Eingabeaufforderung und wechsle in den Ordner `c:\docs\sql.magellan.de\v11`.

2. Tippe den Befehl `mkdocs build` ein. Die Dokumentation wird neu generiert.

3. Um Dir das Ergebnis anzeigen zu lassen, tippe den Befehl `mkdocs serve` ein und öffne die Url `http://127.0.0.1:8000` in Deinem Webbrowser.

Das Inhaltsverzeichnis findest Du in der Datei `mkdocs.yml`, die einzelnen Kapitel im Unterordner `docs`. 

## Kann ich mithelfen?

Ja, sehr gerne. Der beste Weg mitzuhelfen ist es, Rückmeldung per Issue-Tracker zu geben und/oder Korrekturen per Pull-Request zu übermitteln.
