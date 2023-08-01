# Table **MandantenSchulformen**

## Columns

This table contains 4 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Schulformen](../../tables/schulformen)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primary key

This table has a primary key.

**`MandantenSchulformen`**

:   `Mandant, Schulform`

## Foreign keys

This table has one foreign key.

**`FK_MANDANTENSCHULFORMEN_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_MANDANTENSCHULFORMEN_FORM`**

:   `Schulform` » [`Schulformen (Kuerzel)`](../../tables/schulformen) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_MANDANTENSCHULFORMEN_FORM`**

:   `Schulform`

**`FK_MANDANTENSCHULFORMEN_MANDANT`**

:   `Mandant`

**`PK_MANDANTENSCHULFORMEN`**

:   `Mandant, Schulform`
