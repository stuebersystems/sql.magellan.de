# Tabelle **BetriebeBildungsgaenge**

## Spalten

Diese Tabelle hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Betrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Betriebe](../../tables/betriebe)

**`Bildungsgang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Bildungsgaenge](../../tables/bildungsgaenge)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`BetriebeBildungsgaenge`**

:   `Mandant, Betrieb, Bildungsgang`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_BETRIEBEBG_BILDUNGSGANG`**

:   `Bildungsgang` » [`Bildungsgaenge (Kuerzel)`](../../tables/bildungsgaenge) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_BETRIEBEBG_BETRIEB`**

:   `Betrieb, Mandant` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_BETRIEBEBG_BETRIEB`**

:   `Mandant, Betrieb`

**`FK_BETRIEBEBG_BILDUNGSGANG`**

:   `Bildungsgang`

**`PK_BETRIEBEBILDUNGSGAENGE`**

:   `Mandant, Betrieb, Bildungsgang`
