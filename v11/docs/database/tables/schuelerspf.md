# Tabelle **SchuelerSPF**

## Spalten

Diese Tabelle hat 9 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Sportfeste](../../tables/sportfeste)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Sportfest`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Sportfeste](../../tables/sportfeste)

**`Riege`**

:   [`VARCHAR(4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Punktzahl`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Note`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`UrkundeAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Wert | Beschreibung
    - | -
    0 | Keine Urkunde
    1 | Siegerurkunde
    2 | Ehrenurkunde

**`Meldungen`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerSPF`**

:   `Mandant, Schueler, Sportfest`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_SCHUELERSPF_SPORTFEST`**

:   `Mandant, Sportfest` » [`Sportfeste (Kuerzel, Mandant)`](../../tables/sportfeste) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERSPF_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_SCHUELERSPF_SCHUELER`**

:   `Mandant, Schueler`

**`FK_SCHUELERSPF_SPORTFEST`**

:   `Mandant, Sportfest`

**`PK_SCHUELERSPF`**

:   `Mandant, Schueler, Sportfest`
