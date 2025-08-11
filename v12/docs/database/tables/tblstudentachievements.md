# Tabelle **tblStudentAchievements**

## Spalten

Diese Tabelle hat 10 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`StudentTerm`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`Grade`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [GradeEntries](../../tables/gradeentries)

**`GradeFactor`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Report`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`AchievementProfile`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`tblStudentAchievements`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 3 Fremdschlüssel.

**`FK_SA_GRADES`**

:   `Grade, Mandant` » [`GradeEntries (ID, Mandant)`](../../tables/gradeentries) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SA_STUDENTTERM`**

:   `Mandant, StudentTerm` » [`SchuelerZeitraeume (ID, Mandant)`](../../tables/schuelerzeitraeume) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_SA_ACHIEVEMENTPROFILE`**

:   `AchievementProfile, Mandant` » [`AchievementProfiles (ID, Mandant)`](../../tables/achievementprofiles) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 4 Indizes.

**`FK_SA_ACHIEVEMENTPROFILE`**

:   `Mandant, AchievementProfile`

**`FK_SA_GRADES`**

:   `Mandant, Grade`

**`FK_SA_STUDENTTERM`**

:   `Mandant, StudentTerm`

**`PK_STUDENTACHIEVEMENTS`**

:   `Mandant, ID`
