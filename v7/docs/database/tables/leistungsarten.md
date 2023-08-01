# Table **Leistungsarten**

## Columns

This table contains 3 columns.

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Bezeichnung`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Bezeichnung

**`Art`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Art der Leistung

    Value | Description
    - | -
    0 | Schriftlich
    1 | Mündlich
    2 | Praktisch

## Primary key

This table has a primary key.

**`Leistungsarten`**

:   `Kuerzel`

## Indices

This table has one index.

**`PK_LEISTUNGSARTEN`**

:   `Kuerzel`
