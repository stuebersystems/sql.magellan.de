# Table **Zeugnisbeurteilungen**

## Columns

This table contains 3 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Beurteilung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primary key

This table has a primary key.

**`Zeugnisbeurteilungen`**

:   `Mandant, Kuerzel`

## Foreign keys

This table has one foreign key.

**`FK_ZEUGNISBEU_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 2 indices.

**`FK_ZEUGNISBEU_MANDANT`**

:   `Mandant`

**`PK_ZEUGNISBEURTEILUNGEN`**

:   `Mandant, Kuerzel`
