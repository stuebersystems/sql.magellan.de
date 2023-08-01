# Table **Standorte**

## Columns

This table contains 4 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung

**`Gebaeude`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Gebaeude](../../tables/gebaeude)

## Primary key

This table has a primary key.

**`Standorte`**

:   `Mandant, Kuerzel`

## Foreign keys

This table has one foreign key.

**`FK_STANDORT_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_STANDORT_GEBAEUDE`**

:   `Gebaeude, Mandant` » [`Gebaeude (Kuerzel, Mandant)`](../../tables/gebaeude) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

## Indices

This table has 3 indices.

**`FK_STANDORT_GEBAEUDE`**

:   `Mandant, Gebaeude`

**`FK_STANDORT_MANDANT`**

:   `Mandant`

**`PK_STANDORTE`**

:   `Mandant, Kuerzel`
