# Tabelle **BetriebeBerufe**

## Spalten

Diese Tabelle hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Betriebe](../../tables/betriebe)

**`Betrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Betriebe](../../tables/betriebe)

**`Beruf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Berufe](../../tables/berufe)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`BetriebeBerufe`**

:   `Mandant, Betrieb, Beruf`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_BETRIEBEBR_BETRIEB`**

:   `Betrieb, Mandant` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_BETRIEBEBR_BERUF`**

:   `Beruf` » [`Berufe (Kuerzel)`](../../tables/berufe) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_BETRIEBEBR_BERUF`**

:   `Beruf`

**`FK_BETRIEBEBR_BETRIEB`**

:   `Mandant, Betrieb`

**`PK_BETRIEBEBERUFE`**

:   `Mandant, Betrieb, Beruf`
