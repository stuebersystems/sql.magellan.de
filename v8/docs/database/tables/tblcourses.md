# Table **tblCourses**

## Columns

This table contains 14 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Term`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Subject`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`SubjectStatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachstati](../../tables/fachstati)

**`SubjectType`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`SubjectTeacher`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Focus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachschwerpunkte](../../tables/fachschwerpunkte)

**`Level`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [FachNiveaus](../../tables/fachniveaus)

**`CourseNo`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Kursnummer

**`Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Attribute`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Merkmal

## Primary key

This table has a primary key.

**`tblCourses`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_COURSE_FOCUS`**

:   `Focus` » [`Fachschwerpunkte (Kuerzel)`](../../tables/fachschwerpunkte) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_COURSE_LEVEL`**

:   `Level` » [`FachNiveaus (Kuerzel)`](../../tables/fachniveaus) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_COURSE_SUBJECT`**

:   `Mandant, Subject` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_COURSE_SUBJECTSTATUS`**

:   `SubjectStatus` » [`Fachstati (Kuerzel)`](../../tables/fachstati) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_COURSE_SUBJECTTYPE`**

:   `SubjectType` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_COURSE_TERM`**

:   `Term` » [`Zeitraeume (ID)`](../../tables/zeitraeume) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

## Indices

This table has 8 indices.

**`FK_COURSE_BILINGUAL`**

:   `Bilingual`

**`FK_COURSE_FOCUS`**

:   `Focus`

**`FK_COURSE_LEVEL`**

:   `Level`

**`FK_COURSE_SUBJECT`**

:   `Mandant, Subject`

**`FK_COURSE_SUBJECTSTATUS`**

:   `SubjectStatus`

**`FK_COURSE_SUBJECTTYPE`**

:   `SubjectType`

**`FK_COURSE_TERM`**

:   `Term`

**`PK_COURSES`**

:   `Mandant, ID`
