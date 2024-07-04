# Änderungen der Datenstruktur

Dokumentierte Änderungen von Magellan 10 auf 11.

## Tabellen

### Neue Felder

Tabelle                                                                    | Feldname                 | Typ            | Verweis auf
-------------------------------------------------------------------------- | ------------------------ | -------------- | -----------
[AchievementProfiles](../database/tables/achievementprofiles/)             | `Position`               | `VARCHAR(100)` |
[KlassenZeitraeume](../database/tables/klassenzeitraeume/)                 | `Klassensprecher3`       | `INTEGER`      | [Schueler](../database/tables/schueler/)
[KlassenZeitraeume](../database/tables/klassenzeitraeume/)                 | `Klassenelternsprecher3` | `INTEGER`      | [Sorgeberechtigte](../database/tables/sorgeberechtigte/)
[Schueler](../database/tables/schueler/)                                   | `Rufname`                | `VARCHAR(100)` |
[SchuelerFachdaten](../database/tables/schuelerfachdaten/)                 | `EndnoteVorzeitraum`     | `INTEGER`      | [Noten](../database/tables/noten/) 
[tblAuswahlPruefungslisten](../database/tables/tblauswahlpruefungslisten/) | `Lehrer`                 | `INTEGER`      | [tblLehrer](../database/tables/tbllehrer/)

## Gelöschte Felder

Tabelle                                                                    | Feldname
-------------------------------------------------------------------------- | --------
[MedienExemplare](../database/tables/medienexemplare/)                     | `Code128`
[MedienExemplare](../database/tables/medienexemplare/)                     | `Code128Print`

MedienExemplare

## Ansichten

### Neu

Ansicht                                                                         | Beschreibung
------------------------------------------------------------------------------- | ------------
[WortersetzungenVerhaeltnisse](../database/views/wortersetzungenverhaeltnisse/) | Neue Hilfsansicht

### Neue Felder

Ansicht                                                                         | Feldname            | Typ            | Verweis auf
------------------------------------------------------------------------------- | ------------------- | -------------- | -----------
[AuswahlPruefungslisten](../database/views/auswahlpruefungslisten/)             | `Lehrer`            | `INTEGER`      | [tblLehrer](../database/tables/tbllehrer/)
[Schueler2](../database/views/schueler2/)                                       | `Rufname`           | `VARCHAR(100)` |
[SchuelerAnsicht](../database/views/schueleransicht/)                           | `Rufname`           | `VARCHAR(100)` |
