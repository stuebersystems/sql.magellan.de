# Tabelle **Haushaltsstellen**

## Spalten

Diese Tabelle hat 10 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Haushaltstitel](../../tables/haushaltstitel)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Haushaltstitel`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Haushaltstitel](../../tables/haushaltstitel)

**`Kuerzel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

**`Bezeichnung`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Gewichtung`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Restuebernahme`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Verwalter`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Gesamtbetrag`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`SummeBuchungen`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Haushaltsstellen`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_HAUSHALTSSTELLEN_TITEL`**

:   `Haushaltstitel, Mandant` » [`Haushaltstitel (ID, Mandant)`](../../tables/haushaltstitel) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_HAUSHALTSSTELLEN_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_HAUSHALTSSTELLEN_MANDANT`**

:   `Mandant`

**`FK_HAUSHALTSSTELLEN_TITEL`**

:   `Mandant, Haushaltstitel`

**`PK_HAUSHALTSSTELLEN`**

:   `Mandant, ID`
