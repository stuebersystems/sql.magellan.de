# Table **SchuelerZeugnisformulare**

## Columns

This table contains 8 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Formular`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`Typ`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

## Primary key

This table has a primary key.

**`SchuelerZeugnisformulare`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_SZF_TERM`**

:   `Mandant, SchuelerZeitraumID` » [`SchuelerZeitraeume (ID, Mandant)`](../../tables/schuelerzeitraeume) · `ON UPDATE NO ACTION` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_SCHUELERZEUGNISFRM_FORMULAR`**

:   `Mandant, Formular`

**`FK_SZF_TERM`**

:   `Mandant, SchuelerZeitraumID`

**`PK_SCHUELERZEUGNISFRM`**

:   `Mandant, ID`
