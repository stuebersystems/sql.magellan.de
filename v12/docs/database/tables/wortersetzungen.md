# Tabelle **Wortersetzungen**

## Spalten

Diese Tabelle hat 6 Spalten.

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Eindeutige ID

**`Land`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Ansicht`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Ansicht, auf die sich die Wortersetzungen bezieht

**`BezeichnungOriginal`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Bezeichnung im Original

**`BezeichnungAlternativ`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Neue Bezeichnung

**`Modul`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Schulverwaltung
    1 | Haushalt & Inventar

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Wortersetzungen`**

:   `ID`

## Indizes

Diese Tabelle hat einen Index.

**`PK_WORTERSETZUNGEN`**

:   `ID`
