# Table **StudentCourseAttendance**

## Columns

This table contains 8 columns.

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

**`ClassCourse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [tblCourses](../../tables/tblcourses)

**`ForgotHomework`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Hausaufgaben vergessen?

**`ForgotMaterial`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Arbeitsmittel vergessen?

## Primary key

This table has a primary key.

**`StudentCourseAttendance`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_STUDENTCOURSEATT_STUDENTTERM`**

:   `Mandant, StudentTerm` » [`SchuelerZeitraeume (ID, Mandant)`](../../tables/schuelerzeitraeume) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_STUDENTCOURSEATT_CLASSCOURSE`**

:   `ClassCourse, Mandant` » [`tblClassCourses (ID, Mandant)`](../../tables/tblclasscourses) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_STUDENTCOURSEATT_CLASSCOURSE`**

:   `Mandant, ClassCourse`

**`FK_STUDENTCOURSEATT_STUDENTTERM`**

:   `Mandant, StudentTerm`

**`PK_STUDENTCOURSEATT`**

:   `Mandant, ID`
