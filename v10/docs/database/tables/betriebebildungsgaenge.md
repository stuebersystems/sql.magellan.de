# Table **BetriebeBildungsgaenge**

## Columns

This table contains 3 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Betrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Betriebe](../../tables/betriebe)

**`Bildungsgang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Bildungsgaenge](../../tables/bildungsgaenge)

## Primary key

This table has a primary key.

**`BetriebeBildungsgaenge`**

:   `Mandant, Betrieb, Bildungsgang`

## Foreign keys

This table has one foreign key.

**`FK_BETRIEBEBG_BILDUNGSGANG`**

:   `Bildungsgang` » [`Bildungsgaenge (Kuerzel)`](../../tables/bildungsgaenge) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_BETRIEBEBG_BETRIEB`**

:   `Betrieb, Mandant` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_BETRIEBEBG_BETRIEB`**

:   `Mandant, Betrieb`

**`FK_BETRIEBEBG_BILDUNGSGANG`**

:   `Bildungsgang`

**`PK_BETRIEBEBILDUNGSGAENGE`**

:   `Mandant, Betrieb, Bildungsgang`
