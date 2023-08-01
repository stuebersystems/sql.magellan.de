# Tabelle **Leistungsarten**

## Spalten

Diese Tabelle hat 3 Spalten.

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Bezeichnung`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Bezeichnung

**`Art`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Art der Leistung

    Wert | Beschreibung
    - | -
    0 | Schriftlich
    1 | Mündlich
    2 | Praktisch

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Leistungsarten`**

:   `Kuerzel`

## Indizes

Diese Tabelle hat einen Index.

**`PK_LEISTUNGSARTEN`**

:   `Kuerzel`
