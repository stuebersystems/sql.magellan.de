# Änderungen der Datenstruktur

Dokumentierte Änderungen von MAGELLAN 7 auf 8.

## Tabellen

### Neue Tabellen

Tabelle                                                              | Beschreibung
-------------------------------------------------------------------- | ------------
[Besonderheiten](../database/tables/besonderheiten/)                 | Ein Schlüsselverzeichnis zum Speichern von Besonderheiten (Text unbestimmter Länger) für Schüler oder Klassen
[KlassenBesonderheiten](../database/tables/klassenbesonderheiten/)   | Verwaltet eine Liste von Besonderheiten für eine Klasse. Besonderheiten können entweder aus dem Schlüsselverzeichnis kopiert oder frei eingetragen werden
[SchuelerBesonderheiten](../database/tables/schuelerbesonderheiten/) | Verwaltet eine Liste von Besonderheiten für einen Schüler. Besonderheiten können entweder aus dem Schlüsselverzeichnis kopiert oder frei eingetragen werden
[tblBenutzerRechte](../database/tables/tblbenutzerrechte/)           | Neue Tabelle für Benutzerrechte

### Neue Felder

Tabelle                                                              | Feldname                          | Verweis auf           | Typ
-------------------------------------------------------------------- | --------------------------------- | --------------------- | ---
[BetriebeKontakte](../database/tables/betriebekontakte/)             | `Anrede`                          |                       | `CHAR(1)`
[Faecher](../database/tables/faecher/)                               | `Bezeichnung3`                    |                       | `VARCHAR(300)`
[KlassenZeitraeume](../database/tables/klassenzeitraeume/)           | `GUIDExtern`                      |                       | `VARCHAR(40)`
[KlassenZeitraeume](../database/tables/klassenzeitraeume/)           | `GUIDExtern`                      |                       | `VARCHAR(40)`
[Kurssprachen](../database/tables/kurssprachen/)                     | `Bezeichnung3`                    |                       | `VARCHAR(300)`
[MedienExemplare](../database/tables/medienexemplare/)               | `Code128Print`                    |                       | `VARCHAR(50)`
[MedienExemplare](../database/tables/medienexemplare/)               | `Code128`                         |                       | `VARCHAR(50)`
[SchuelerFachdaten](../database/tables/schuelerfachdaten/)           | `GUIDExtern`                      |                       | `VARCHAR(40)`
[SchuelerFachdaten](../database/tables/schuelerfachdaten/)           | `Thema`                           |                       | `BLOB subtype text`
[SchuelerSorgebe](../database/tables/schuelersorgebe/)               | `Hauptversicherter`               |                       | `CHAR(1)`
[Schueler](../database/tables/schueler/)                             | `HoechsterAbschluss2ABSSchulform` | `SchulformenHerkunft` | `VARCHAR(20)`
[Schueler](../database/tables/schueler/)                             | `HoechsterAbschluss2ABS`          | `AbschluesseExtern`   | `VARCHAR(20)`
[Schueler](../database/tables/schueler/)                             | `HoechsterAbschluss2BBSSchulform` | `SchulformenHerkunft` | `VARCHAR(20)`
[Schueler](../database/tables/schueler/)                             | `HoechsterAbschluss2BBS`          | `AbschluesseExtern`   | `VARCHAR(20)`
[Schueler](../database/tables/schueler/)                             | `MerkmalA7`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Schueler](../database/tables/schueler/)                             | `MerkmalA8`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Schueler](../database/tables/schueler/)                             | `MerkmalA9`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Schueler](../database/tables/schueler/)                             | `MerkmalA10`                      | `SchuelerMerkmale`    | `VARCHAR(20)`
[Staatsangehoerigkeiten](../database/tables/staatsangehoerigkeiten/) | `Bezeichnung2`                    |                       | `VARCHAR(300)`
[Zeugnisbemerkungen](../database/tables/zeugnisbemerkungen/)         | `Fortschreiben`                   |                       | `CHAR(1)`

### Geänderte Felder

Tabelle                                               | Feldname             | Änderung
----------------------------------------------------- | -------------------- | --------
[SchuelerABI2](../database/tables/schuelerabi2/)      | `LernleistungThema`  | Feldgröße erweitert auf 300
[SchuelerABI2](../database/tables/schuelerabi2/)      | `PraesentationThema` | Feldgröße erweitert auf 300
[SchuelerABI2](../database/tables/schuelerabi2/)      | `ProjektThema`       | Feldgröße erweitert auf 300
[SchuelerABI](../database/tables/schuelerabi/)        | `LernleistungThema`  | Feldgröße erweitert auf 300
[SchuelerABI](../database/tables/schuelerabi/)        | `PraesentationThema` | Feldgröße erweitert auf 300
[SchuelerABI](../database/tables/schuelerabi/)        | `ProjektThema`       | Feldgröße erweitert auf 300
[Schueler](../database/tables/schueler/)              | `BewerberStatus`     | Neuer Wert: `13 - Ablehnungsbescheid`

## Ansichten

### Neue Ansichten

Ansicht                                                              | Beschreibung
-------------------------------------------------------------------- | ------------
[BenutzerRechte](../database/tables/benutzerrechte/)                 | Neue Ansicht für Benutzerrechte

### Neue Felder

Ansicht                                                              | Feldname                          | Verweis auf           | Typ
-------------------------------------------------------------------- | --------------------------------- | --------------------- | ---
[Schueler2](../database/views/schueler2/)                            | `HoechsterAbschluss2ABSSchulform` | `SchulformenHerkunft` | `VARCHAR(20)`
[Schueler2](../database/views/schueler2/)                            | `HoechsterAbschluss2ABS`          | `AbschluesseExtern`   | `VARCHAR(20)`
[Schueler2](../database/views/schueler2/)                            | `HoechsterAbschluss2BBSSchulform` | `SchulformenHerkunft` | `VARCHAR(20)`
[Schueler2](../database/views/schueler2/)                            | `HoechsterAbschluss2BBS`          | `AbschluesseExtern`   | `VARCHAR(20)`
[Schueler2](../database/tables/schueler2/)                           | `MerkmalA7`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Schueler2](../database/tables/schueler2/)                           | `MerkmalA8`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Schueler2](../database/tables/schueler2/)                           | `MerkmalA9`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Schueler2](../database/tables/schueler2/)                           | `MerkmalA10`                      | `SchuelerMerkmale`    | `VARCHAR(20)`
[SchuelerAnsicht](../database/views/schueleransicht/)                | `HoechsterAbschluss2ABSSchulform` | `SchulformenHerkunft` | `VARCHAR(20)`
[SchuelerAnsicht](../database/views/schueleransicht/)                | `HoechsterAbschluss2ABS`          | `AbschluesseExtern`   | `VARCHAR(20)`
[SchuelerAnsicht](../database/views/schueleransicht/)                | `HoechsterAbschluss2BBSSchulform` | `SchulformenHerkunft` | `VARCHAR(20)`
[SchuelerAnsicht](../database/views/schueleransicht/)                | `HoechsterAbschluss2BBS`          | `AbschluesseExtern`   | `VARCHAR(20)`
[SchuelerFamilie](../database/views/schuelerfamilie/)                | `Hauptversicherter`               |                       | `CHAR(1)`
[Vagabonds](../database/views/vagabonds/)                            | `MerkmalA7`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Vagabonds](../database/views/vagabonds/)                            | `MerkmalA8`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Vagabonds](../database/views/vagabonds/)                            | `MerkmalA9`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[Vagabonds](../database/views/vagabonds/)                            | `MerkmalA10`                      | `SchuelerMerkmale`    | `VARCHAR(20)`
[SchuelerAbwesenheiten](../database/views/schuelerabwesenheiten/)    | `HoechsterAbschluss2ABSSchulform` | `SchulformenHerkunft` | `VARCHAR(20)`
[SchuelerAbwesenheiten](../database/views/schuelerabwesenheiten/)    | `HoechsterAbschluss2ABS`          | `AbschluesseExtern`   | `VARCHAR(20)`
[SchuelerAbwesenheiten](../database/views/schuelerabwesenheiten/)    | `HoechsterAbschluss2BBSSchulform` | `SchulformenHerkunft` | `VARCHAR(20)`
[SchuelerAbwesenheiten](../database/views/schuelerabwesenheiten/)    | `HoechsterAbschluss2BBS`          | `AbschluesseExtern`   | `VARCHAR(20)`
[SchuelerAbwesenheiten](../database/views/schuelerabwesenheiten/)    | `MerkmalA7`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[SchuelerAbwesenheiten](../database/views/schuelerabwesenheiten/)    | `MerkmalA8`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[SchuelerAbwesenheiten](../database/views/schuelerabwesenheiten/)    | `MerkmalA9`                       | `SchuelerMerkmale`    | `VARCHAR(20)`
[SchuelerAbwesenheiten](../database/views/schuelerabwesenheiten/)    | `MerkmalA10`                      | `SchuelerMerkmale`    | `VARCHAR(20)`

### Geänderte Felder

Ansicht                                               | Feldname             | Änderung
----------------------------------------------------- | -------------------- | --------
[Schueler2](../database/views/schueler2/)             | `BewerberStatus`     | Neuer Wert: `13 - Ablehnungsbescheid`
[SchuelerAnsicht](../database/views/schueleransicht/) | `BewerberStatus`     | Neuer Wert: `13 - Ablehnungsbescheid`
[Vagabonds](../database/views/vagabonds/)             | `BewerberStatus`     | Neuer Wert: `13 - Ablehnungsbescheid`