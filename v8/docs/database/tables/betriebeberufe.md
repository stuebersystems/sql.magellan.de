# Table **BetriebeBerufe**

## Columns

This table contains 3 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Betriebe](../../tables/betriebe)

**`Betrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Betriebe](../../tables/betriebe)

**`Beruf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Berufe](../../tables/berufe)

## Primary key

This table has a primary key.

**`BetriebeBerufe`**

:   `Mandant, Betrieb, Beruf`

## Foreign keys

This table has one foreign key.

**`FK_BETRIEBEBR_BETRIEB`**

:   `Betrieb, Mandant` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_BETRIEBEBR_BERUF`**

:   `Beruf`

**`FK_BETRIEBEBR_BETRIEB`**

:   `Mandant, Betrieb`

**`PK_BETRIEBEBERUFE`**

:   `Mandant, Betrieb, Beruf`
