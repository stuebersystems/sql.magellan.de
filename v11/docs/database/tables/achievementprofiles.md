# Tabelle **AchievementProfiles**

## Spalten

Diese Tabelle hat 15 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [GradeTypes](../../tables/gradetypes)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Configuration`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Grade
    1 | Report
    2 | Grade and Report
    3 | ComplexReport

**`GradeSystem`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [GradeSystems](../../tables/gradesystems)

**`GradeType`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [GradeTypes](../../tables/gradetypes)

**`AssessmentProfile`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [AssessmentProfiles](../../tables/assessmentprofiles)

**`ClassTerm`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [KlassenZeitraeume](../../tables/klassenzeitraeume)

**`Course`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblCourses](../../tables/tblcourses)

**`Code`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Kürzel für Leistungsprofil

**`Name`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung

**`Description`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Beschreibung

**`InternalCode`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Interner Code\. Mögliche Werte werden zukünftig noch festgelegt

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`AchievementProfiles`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 5 Fremdschlüssel.

**`FK_ACHIEVEPROFILE_CLASSTERM`**

:   `ClassTerm, Mandant` » [`KlassenZeitraeume (ID, Mandant)`](../../tables/klassenzeitraeume) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_ACHIEVEPROFILE_COURSE`**

:   `Course, Mandant` » [`tblCourses (ID, Mandant)`](../../tables/tblcourses) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_ACHIEVEPROFILE_GRADESYSTEM`**

:   `GradeSystem, Mandant` » [`GradeSystems (ID, Mandant)`](../../tables/gradesystems) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_ACHIEVEPROFILE_GRADETYPE`**

:   `GradeType, Mandant` » [`GradeTypes (ID, Mandant)`](../../tables/gradetypes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_ACHIEVEPROFILE_ASSMPROFILE`**

:   `AssessmentProfile, Mandant` » [`AssessmentProfiles (ID, Mandant)`](../../tables/assessmentprofiles) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 6 Indizes.

**`FK_ACHIEVEPROFILE_ASSMPROFILE`**

:   `Mandant, AssessmentProfile`

**`FK_ACHIEVEPROFILE_CLASSTERM`**

:   `Mandant, ClassTerm`

**`FK_ACHIEVEPROFILE_COURSE`**

:   `Mandant, Course`

**`FK_ACHIEVEPROFILE_GRADESYSTEM`**

:   `Mandant, GradeSystem`

**`FK_ACHIEVEPROFILE_GRADETYPE`**

:   `Mandant, GradeType`

**`PK_ACHIEVEMENTPROFILES`**

:   `Mandant, ID`
