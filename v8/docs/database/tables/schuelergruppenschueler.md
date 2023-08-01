# Table **SchuelergruppenSchueler**

## Columns

This table contains 5 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Schuelergruppe`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`Zugang`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Abgang`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

## Primary key

This table has a primary key.

**`SchuelergruppenSchueler`**

:   `Mandant, Schueler, Schuelergruppe`

## Foreign keys

This table has one foreign key.

**`FK_SGRUPPENSCHUELER_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_SGRUPPENSCHUELER_GRUPPE`**

:   `Mandant, Schuelergruppe`

**`FK_SGRUPPENSCHUELER_SCHUELER`**

:   `Mandant, Schueler`

**`PK_SGRUPPENSCHUELER`**

:   `Mandant, Schueler, Schuelergruppe`
