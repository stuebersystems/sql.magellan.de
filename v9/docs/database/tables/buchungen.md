# Table **Buchungen**

## Columns

This table contains 18 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Haushaltsstelle`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Haushaltsstellen](../../tables/haushaltsstellen)

**`Buchungsart`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Ausgabe
    1 | Einnahme
    2 | Ausgabe\-Korrektur
    3 | Einnahme\-Korrektur
    4 | Geplante Ausgabe

**`Bereich`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Buchungsbereiche](../../tables/buchungsbereiche)

**`Datum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime) · `NOT NULL`

**`Betrag`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes) · `NOT NULL`

**`Grund`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`BelegNr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Besteller`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BestellNr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BestellDatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`RechnungNr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`LieferscheinNr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Lieferant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Lieferanten](../../tables/lieferanten)

**`Log_Datum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Log_Uhrzeit`**

:   [`TIME`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Log_Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primary key

This table has a primary key.

**`Buchungen`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_BUCHUNGEN_HAUSHALTSSTELLE`**

:   `Haushaltsstelle, Mandant` » [`Haushaltsstellen (ID, Mandant)`](../../tables/haushaltsstellen) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_BUCHUNGEN_LIEFERANT`**

:   `Lieferant` » [`Lieferanten (ID)`](../../tables/lieferanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_BUCHUNGEN_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

## Indices

This table has 5 indices.

**`FK_BUCHUNGEN_BEREICH`**

:   `Mandant, Bereich`

**`FK_BUCHUNGEN_HAUSHALTSSTELLE`**

:   `Mandant, Haushaltsstelle`

**`FK_BUCHUNGEN_LIEFERANT`**

:   `Lieferant`

**`FK_BUCHUNGEN_MANDANT`**

:   `Mandant`

**`PK_BUCHUNGEN`**

:   `Mandant, ID`
