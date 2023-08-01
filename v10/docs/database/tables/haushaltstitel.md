# Table **Haushaltstitel**

## Columns

This table contains 10 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Kuerzel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

**`Bezeichnung`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Haushalt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

**`Haushaltsjahr`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Haushaltsjahre](../../tables/haushaltsjahre)

**`Restuebernahme`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Gesamtbetrag`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`SummeHaushaltsstellen`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`SummeBuchungen`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

## Primary key

This table has a primary key.

**`Haushaltstitel`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_HAUSHALTSTITEL_JAHR`**

:   `Haushaltsjahr, Mandant` » [`Haushaltsjahre (Kuerzel, Mandant)`](../../tables/haushaltsjahre) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_HAUSHALTSTITEL_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_HAUSHALTSTITEL_HAUSHALT`**

:   `Haushalt` » [`Haushalte (Kuerzel)`](../../tables/haushalte) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

## Indices

This table has 4 indices.

**`FK_HAUSHALTSTITEL_HAUSHALT`**

:   `Haushalt`

**`FK_HAUSHALTSTITEL_JAHR`**

:   `Mandant, Haushaltsjahr`

**`FK_HAUSHALTSTITEL_MANDANT`**

:   `Mandant`

**`PK_HAUSHALTSTITEL`**

:   `Mandant, ID`
