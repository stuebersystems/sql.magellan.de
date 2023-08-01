# Tabelle **tblClassCourses**

Grundlage sind die Tabellen [KlassenZeitraeume](../../tables/klassenzeitraeume), [tblClassCourses](../../tables/tblclasscourses) und [tblCourses](../../tables/tblcourses)

## Spalten

Diese Tabelle hat 6 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [tblCourses](../../tables/tblcourses)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`ClassTerm`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`Course`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [tblCourses](../../tables/tblcourses)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`tblClassCourses`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_CLASSCOURSE_COURSE`**

:   `Course, Mandant` » [`tblCourses (ID, Mandant)`](../../tables/tblcourses) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_CLASSCOURSE_CLASSTERM`**

:   `Mandant, ClassTerm`

**`FK_CLASSCOURSE_COURSE`**

:   `Mandant, Course`

**`PK_CLASSCOURSES`**

:   `Mandant, ID`
