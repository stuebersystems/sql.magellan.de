# Table **SchuelerMerkmale**

## Columns

This table contains 8 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Schluessel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Statistikschlüssel

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung

**`Bereich`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Zuordnung des Merkmals

    Value | Description
    - | -
    0 | Merkmal A1
    1 | Merkmal A2
    2 | Merkmal A3
    3 | Merkmal A4
    4 | Merkmal A5
    5 | Merkmal A6
    6 | Merkmal S1
    7 | Merkmal S2
    8 | Merkmal S3
    9 | Merkmal S4
    10 | Merkmal S5
    11 | Merkmal S6
    12 | Merkmal S7
    13 | Merkmal S8
    14 | Merkmal S9
    15 | Merkmal S10

**`StatistikID`**

:   [`VARCHAR(16)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`GueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig ab

**`GueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig bis

## Primary key

This table has a primary key.

**`SchuelerMerkmale`**

:   `Mandant, Kuerzel`

## Foreign keys

This table has one foreign key.

**`FK_SCHUELERMERKMALE_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 2 indices.

**`FK_SCHUELERMERKMALE_MANDANT`**

:   `Mandant`

**`PK_SCHUELERMERKMALE`**

:   `Mandant, Kuerzel`
