# Änderungen der Datenstruktur

Dokumentierte Änderungen von Magellan 8 auf 9.

## Tabellen

### Neu

Tabelle                                                      | Beschreibung
------------------------------------------------------------ | ------------
[FremdsprachenNoten](../database/tables/fremdsprachennoten/) | Neues Schlüsselverzeichnis

### Neue Felder

Tabelle                                                                      | Feldname               | Verweis auf      | Typ 
---------------------------------------------------------------------------- | ---------------------- | ---------------- | ----
[Banken](../database/tables/banken/)                                         | `EnbreaID`             |                  | `VARCHAR(24)`
[Besonderheiten](../database/tables/besonderheiten/)                         | `EnbreaID`             |                  | `VARCHAR(24)`
[BetriebeKontakte](../database/tables/betriebekontakte/)                     | `EnbreaID`             |                  | `VARCHAR(24)`
[KlassenBesonderheiten](../database/tables/klassenbesonderheiten/)           | `EnbreaID`             |                  | `VARCHAR(24)`
[KlassenZeitraeume](../database/tables/klassenzeitraeume/)                   | `EnbreaID`             |                  | `VARCHAR(24)`
[MedienArten](../database/tables/medienarten/)                               | `EnbreaID`             |                  | `VARCHAR(24)`
[MedienExemplare](../database/tables/medienexemplare/)                       | `EnbreaID`             |                  | `VARCHAR(24)`
[MedienKataloge](../database/tables/medienkataloge/)                         | `EnbreaID`             |                  | `VARCHAR(24)`
[MedienVorgaenge](../database/tables/medienvorgaenge/)                       | `EnbreaID`             |                  | `VARCHAR(24)`
[Medien](../database/tables/medien/)                                         | `EnbreaID`             |                  | `VARCHAR(24)`
[MedizinKategorien](../database/tables/medizinkategorien/)                   | `EnbreaID`             |                  | `VARCHAR(24)`
[Noten](../database/tables/noten/)                                           | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerAusbildung](../database/tables/schuelerausbildung/)                 | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerBesonderheiten](../database/tables/schuelerbesonderheiten/)         | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerFachdaten](../database/tables/schuelerfachdaten/)                   | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerFehlzeiten](../database/tables/schuelerfehlzeiten/)                 | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerFoerderungen](../database/tables/schuelerfoerderungen/)             | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerSchulen](../database/tables/schuelerschulen/)                       | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerSorgebe](../database/tables/schuelersorgebe/)                       | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerZeitraeume](../database/tables/schuelerzeitraeume/)                 | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerZeugnisbemerkungen](../database/tables/schuelerzeugnisbemerkungen/) | `EnbreaID`             |                  | `VARCHAR(24)`
[SchuelerZeugnisformulare](../database/tables/schuelerzeugnisformulare/)     | `EnbreaID`             |                  | `VARCHAR(24)`
[Schueler](../database/tables/schueler/)                                     | `Fremdsprache1Erteilt` |                  | `VARCHAR(100)`
[Schueler](../database/tables/schueler/)                                     | `Fremdsprache2Erteilt` |                  | `VARCHAR(100)`
[Schueler](../database/tables/schueler/)                                     | `Fremdsprache2Erteilt` |                  | `VARCHAR(100)`
[Schueler](../database/tables/schueler/)                                     | `Fremdsprache4Erteilt` |                  | `VARCHAR(100)`
[Schulen](../database/tables/schulen/)                                       | `EnbreaID`             |                  | `VARCHAR(24)`
[Sorgeberechtigte](../database/tables/sorgeberechtigte/)                     | `Geschlecht`           |                  | `VARCHAR(100)`
[Zeitraeume](../database/tables/zeitraeume/)                                 | `EnbreaID`             |                  | `VARCHAR(24)`

### Geänderte Felder

Tabelle                                   | Feldname             | Änderung
----------------------------------------- | -------------------- | --------
[Schueler](../database/tables/schueler/)  | `Fremdsprache1Note`  | Neuer Typ: `VARCHAR(20)` mit Verweis auf Tabelle [FremdsprachenNoten](../database/tables/fremdsprachennoten/)
[Schueler](../database/tables/schueler/)  | `Fremdsprache2Note`  | Neuer Typ: `VARCHAR(20)` mit Verweis auf Tabelle [FremdsprachenNoten](../database/tables/fremdsprachennoten/)
[Schueler](../database/tables/schueler/)  | `Fremdsprache3Note`  | Neuer Typ: `VARCHAR(20)` mit Verweis auf Tabelle [FremdsprachenNoten](../database/tables/fremdsprachennoten/)
[Schueler](../database/tables/schueler/)  | `Fremdsprache4Note`  | Neuer Typ: `VARCHAR(20)` mit Verweis auf Tabelle [FremdsprachenNoten](../database/tables/fremdsprachennoten/)

## Ansichten

### Neue Felder

Ansicht                                                                      | Feldname               | Verweis auf      | Typ 
---------------------------------------------------------------------------- | ---------------------- | ---------------- | ----
[SchuelerFamilie](../database/views/schuelerfamilie/)                        | `Geschlecht`           |                  | `VARCHAR(100)`
