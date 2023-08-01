# Table **Statistik**

## Columns

This table contains 6 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`MagellanID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`StatistikID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Merkmal`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Typ`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Value | Description
    - | -
    0 | Lehrer
    1 | Lehrerbeschaeftigung
    2 | LehrerLehraemter
    3 | LehrerVorgaengeReduktionen
    4 | Schueler
    5 | SchuelerFremdprachen
    6 | Schuelerbehinderungsarten
    7 | SchuelerBildungsgaenge
    8 | SchuelerAbschluesse
    9 | SchuelerGrundschulempfehlung
    10 | SchuelerKurswahl
    11 | Adresse
    12 | Betriebe
    13 | Bundesjugendspiele
    14 | SchuelerUebergang
    15 | Lehrerbeschaeftigung

## Primary key

This table has a primary key.

**`Statistik`**

:   `Mandant, ID`

## Indices

This table has one index.

**`PK_Statistik`**

:   `Mandant, ID`
