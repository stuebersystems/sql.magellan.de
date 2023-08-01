# Table **Unterrichtseinheiten**

## Columns

This table contains 12 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`VeranstaltungNr`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`Fachstatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachstati](../../tables/fachstati)

**`Schwerpunkt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachschwerpunkte](../../tables/fachschwerpunkte)

**`KursNr`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Soll`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Sollstunden \(=Soll aus DAVINCI\)

**`Angleichung`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Angleichung \(=Angleichung aus DAVINCI\)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primary key

This table has a primary key.

**`Unterrichtseinheiten`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_UEINHEITEN_FACHSTATUS`**

:   `Fachstatus` » [`Fachstati (Kuerzel)`](../../tables/fachstati) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_UEINHEITEN_KLASSE`**

:   `Klasse, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_UEINHEITEN_SCHWERPUNKT`**

:   `Schwerpunkt` » [`Fachschwerpunkte (Kuerzel)`](../../tables/fachschwerpunkte) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_UEINHEITEN_UNTERRICHTSART`**

:   `Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

## Indices

This table has 6 indices.

**`FK_UEINHEITEN_FACH`**

:   `Mandant, Fach`

**`FK_UEINHEITEN_FACHSTATUS`**

:   `Fachstatus`

**`FK_UEINHEITEN_KLASSE`**

:   `Mandant, Klasse`

**`FK_UEINHEITEN_SCHWERPUNKT`**

:   `Schwerpunkt`

**`FK_UEINHEITEN_UNTERRICHTSART`**

:   `Unterrichtsart`

**`PK_UEINHEITEN`**

:   `Mandant, ID`
