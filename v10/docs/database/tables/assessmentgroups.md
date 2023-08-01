# Table **AssessmentGroups**

## Columns

This table contains 11 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [AssessmentProfiles](../../tables/assessmentprofiles)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Profile`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [AssessmentProfiles](../../tables/assessmentprofiles)

**`Code`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Kürzel für Bewertungsgruppen

**`Name`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung

**`Configuration`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Value | Description
    - | -
    0 | keine Bewertung
    1 | Grade
    2 | Report
    3 | Grade und Report

**`GradeSystem`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [GradeSystems](../../tables/gradesystems)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Description`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Beschreibung

**`InternalCode`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Interner Code\. Mögliche Werte werden zukünftig noch festgelegt

## Primary key

This table has a primary key.

**`AssessmentGroups`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_ASSESSMENTGROUP_PROFILE`**

:   `Mandant, Profile` » [`AssessmentProfiles (ID, Mandant)`](../../tables/assessmentprofiles) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_ASSESSMENTGROUP_GRADESYSTEM`**

:   `GradeSystem, Mandant` » [`GradeSystems (ID, Mandant)`](../../tables/gradesystems) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indices

This table has 3 indices.

**`FK_ASSESSMENTGROUP_GRADESYSTEM`**

:   `Mandant, GradeSystem`

**`FK_ASSESSMENTGROUP_PROFILE`**

:   `Mandant, Profile`

**`PK_ASSESSMENTGROUPS`**

:   `Mandant, ID`
