# Tabelle **Bildungsgaenge**

## Spalten

Diese Tabelle hat 18 Spalten.

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Schluessel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Statistikschlüssel

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung

**`Bezeichnung2`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung 2

**`Berufsfeld`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Berufsfelder](../../tables/berufsfelder)

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schulformen](../../tables/schulformen)

**`Organisation`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Organisationen](../../tables/organisationen)

**`Unterrichtsform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsformen](../../tables/unterrichtsformen)

**`Fachrichtung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachrichtungen](../../tables/fachrichtungen)

**`Schwerpunkt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schwerpunkte](../../tables/schwerpunkte)

**`Schwerpunkt2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schwerpunkte](../../tables/schwerpunkte)

**`Klassenstufe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Klassenstufen](../../tables/klassenstufen)

**`Dauer`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Dauer des Bildungsgangs

**`Qualifikationsniveau`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Qualifikationsniveaus](../../tables/qualifikationsniveaus)

**`StatistikID`**

:   [`VARCHAR(16)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Kategorie`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Interner Schlüssel
    1 | Externer Schlüssel
    2 | Interner und externer Schlüssel

**`GueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig ab

**`GueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig bis

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Bildungsgaenge`**

:   `Kuerzel`

## Fremdschlüssel

Diese Tabelle hat 9 Fremdschlüssel.

**`FK_BILDUNGSGAENGE_FACHRICHTUNG`**

:   `Fachrichtung` » [`Fachrichtungen (Kuerzel)`](../../tables/fachrichtungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_BILDUNGSGAENGE_KLASSENSTUFE`**

:   `Klassenstufe` » [`Klassenstufen (Kuerzel)`](../../tables/klassenstufen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_BILDUNGSGAENGE_ORGANISATION`**

:   `Organisation` » [`Organisationen (Kuerzel)`](../../tables/organisationen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_BILDUNGSGAENGE_QUALI`**

:   `Qualifikationsniveau` » [`Qualifikationsniveaus (Kuerzel)`](../../tables/qualifikationsniveaus) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_BILDUNGSGAENGE_SCHULFORM`**

:   `Schulform` » [`Schulformen (Kuerzel)`](../../tables/schulformen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_BILDUNGSGAENGE_SCHWERPUNKT`**

:   `Schwerpunkt` » [`Schwerpunkte (Kuerzel)`](../../tables/schwerpunkte) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_BILDUNGSGAENGE_SCHWERPUNKT2`**

:   `Schwerpunkt2` » [`Schwerpunkte (Kuerzel)`](../../tables/schwerpunkte) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_BILDUNGSGAENGE_UNTERRICHT`**

:   `Unterrichtsform` » [`Unterrichtsformen (Kuerzel)`](../../tables/unterrichtsformen) · `ON UPDATE SET NULL` · `ON DELETE SET NULL`

**`FK_BILDUNGSGAENGE_BERUFSFELD`**

:   `Berufsfeld` » [`Berufsfelder (Kuerzel)`](../../tables/berufsfelder) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 11 Indizes.

**`FK_BILDUNGSGAENGE_BERUFSFELD`**

:   `Berufsfeld`

**`FK_BILDUNGSGAENGE_FACHRICHTUNG`**

:   `Fachrichtung`

**`FK_BILDUNGSGAENGE_KLASSENSTUFE`**

:   `Klassenstufe`

**`FK_BILDUNGSGAENGE_ORGANISATION`**

:   `Organisation`

**`FK_BILDUNGSGAENGE_QUALI`**

:   `Qualifikationsniveau`

**`FK_BILDUNGSGAENGE_SCHULFORM`**

:   `Schulform`

**`FK_BILDUNGSGAENGE_SCHWERPUNKT`**

:   `Schwerpunkt`

**`FK_BILDUNGSGAENGE_SCHWERPUNKT2`**

:   `Schwerpunkt2`

**`FK_BILDUNGSGAENGE_UNTERRICHT`**

:   `Unterrichtsform`

**`IDX_Bildungsgaenge_Kategorie`**

:   `Kategorie`

**`PK_BILDUNGSGAENGE`**

:   `Kuerzel`
