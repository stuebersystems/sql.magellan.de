# Table **Faecher**

## Columns

This table contains 16 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

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

**`Bezeichnung3`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung 3

**`Kategorie`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Value | Description
    - | -
    0 | Fremdsprache
    1 | Religion\/Ethik
    2 | Deutsch
    3 | Mathematik
    4 | Kunst
    5 | Musik
    6 | Sport
    9 | Informatik
    10 | Philosophie
    11 | Geschichte
    12 | Physik
    13 | Chemie
    14 | Biologie
    15 | Erdkunde
    16 | Sozialkunde
    17 | Wirtschaft
    18 | Politik
    19 | Darstellendes Spiel
    20 | Evangelische Religion
    21 | Katholische Religion
    26 | Technik
    27 | Pädagogik
    28 | Sport\-Theorie
    29 | BWL\/RW
    30 | BWL\/VWL
    31 | VWL
    32 | Seminar
    33 | Gesundheit
    34 | Psychologie
    35 | Recht
    36 | Pädagogik
    37 | Literatur

**`Aufgabenbereich`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Value | Description
    - | -
    0 | sprachl\.\-lit\.\-künstlerisch
    1 | gesellschaftswiss\.
    2 | mathem\.\-nat\.\-technisch
    3 | Religion
    4 | Sport

**`Gruppe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachgruppen](../../tables/fachgruppen)

**`KeinAbgleich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Kein Abgleich mit DAVINCI?

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Zeugnismerkmal`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

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

**`Faecher`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_FAECHER_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 4 indices.

**`FK_FAECHER_GRUPPE`**

:   `Gruppe`

**`FK_FAECHER_MANDANT`**

:   `Mandant`

**`IDX_Faecher_Kuerzel`**

:   `Kuerzel`

**`PK_FAECHER`**

:   `Mandant, ID`
