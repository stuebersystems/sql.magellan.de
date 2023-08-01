# Table **Haushaltsmittel**

## Columns

This table contains 9 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Haushaltstitel](../../tables/haushaltstitel)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Haushaltstitel`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Haushaltstitel](../../tables/haushaltstitel)

**`Haushaltsstelle`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Haushaltsstellen](../../tables/haushaltsstellen)

**`Datum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Betrag`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`Projekt`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Grund`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

## Primary key

This table has a primary key.

**`Haushaltsmittel`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_HAUSHALTSMITTEL_STELLE`**

:   `Haushaltsstelle, Mandant` » [`Haushaltsstellen (ID, Mandant)`](../../tables/haushaltsstellen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_HAUSHALTSMITTEL_TITEL`**

:   `Haushaltstitel, Mandant` » [`Haushaltstitel (ID, Mandant)`](../../tables/haushaltstitel) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 4 indices.

**`FK_HAUSHALTSMITTEL_MANDANT`**

:   `Mandant`

**`FK_HAUSHALTSMITTEL_STELLE`**

:   `Mandant, Haushaltsstelle`

**`FK_HAUSHALTSMITTEL_TITEL`**

:   `Mandant, Haushaltstitel`

**`PK_HAUSHALTSMITTEL`**

:   `Mandant, ID`
