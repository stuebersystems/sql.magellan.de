# Tabelle **Berufe**

## Spalten

Diese Tabelle hat 11 Spalten.

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Schluessel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Statistikschlüssel

**`BezeichnungM`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Männliche Bezeichnung

**`BezeichnungW`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Weibliche Bezeichnung

**`Fachrichtung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachrichtungen](../../tables/fachrichtungen)

**`Qualifikationsniveau`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Qualifikationsniveaus](../../tables/qualifikationsniveaus)

**`Berufsfeld`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Berufsfelder](../../tables/berufsfelder)

**`StatistikID`**

:   [`VARCHAR(16)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Kategorie`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Interne Schlüssel
    1 | Externe Schlüssel
    2 | Interne und externe Schlüssel

**`GueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig ab

**`GueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig bis

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Berufe`**

:   `Kuerzel`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_BERUFE_FACHRICHTUNG`**

:   `Fachrichtung` » [`Fachrichtungen (Kuerzel)`](../../tables/fachrichtungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_BERUFE_QUALI`**

:   `Qualifikationsniveau` » [`Qualifikationsniveaus (Kuerzel)`](../../tables/qualifikationsniveaus) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 6 Indizes.

**`FK_BERUFE_BERUFSFELD`**

:   `Berufsfeld`

**`FK_BERUFE_FACHRICHTUNG`**

:   `Fachrichtung`

**`FK_BERUFE_QUALI`**

:   `Qualifikationsniveau`

**`IDX_Berufe_Berufsfeld`**

:   `Berufsfeld`

**`IDX_Berufe_Kategorie`**

:   `Kategorie`

**`PK_BERUFE`**

:   `Kuerzel`
