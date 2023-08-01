# Table **tblStudentComplexReports**

## Columns

This table contains 10 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [AssessmentProfiles](../../tables/assessmentprofiles)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`StudentAchievement`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`Profile`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [AssessmentProfiles](../../tables/assessmentprofiles)

**`Group`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [AssessmentGroups](../../tables/assessmentgroups)

**`Entry`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Grade`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [GradeEntries](../../tables/gradeentries)

**`Report`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    Beurteilung

## Primary key

This table has a primary key.

**`tblStudentComplexReports`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_COMPLEXREPORTS_GRADE`**

:   `Grade, Mandant` » [`GradeEntries (ID, Mandant)`](../../tables/gradeentries) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_COMPLEXREPORTS_GROUP`**

:   `Group, Mandant` » [`AssessmentGroups (ID, Mandant)`](../../tables/assessmentgroups) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_COMPLEXREPORTS_PROFILE`**

:   `Mandant, Profile` » [`AssessmentProfiles (ID, Mandant)`](../../tables/assessmentprofiles) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_COMPLEXREPORTS_ENTRY`**

:   `Entry, Mandant` » [`AssessmentEntries (ID, Mandant)`](../../tables/assessmententries) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indices

This table has 5 indices.

**`FK_COMPLEXREPORTS_ENTRY`**

:   `Mandant, Entry`

**`FK_COMPLEXREPORTS_GRADE`**

:   `Mandant, Grade`

**`FK_COMPLEXREPORTS_GROUP`**

:   `Mandant, Group`

**`FK_COMPLEXREPORTS_PROFILE`**

:   `Mandant, Profile`

**`PK_COMPLEXREPORTS`**

:   `Mandant, ID`
