# Tabelle **SchuelerZeugnisbemerkungen**

## Spalten

Diese Tabelle hat 10 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Fortschreiben`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerZeugnisbemerkungen`**

:   `Mandant, ID`

## Indizes

Diese Tabelle hat 2 Indizes.

**`FK_SZB_SCHUELERZEITR`**

:   `Mandant, SchuelerZeitraumID`

**`PK_SCHUELERZGNBEMERK`**

:   `Mandant, ID`
