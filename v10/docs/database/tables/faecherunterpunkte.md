# Table **FaecherUnterpunkte**

## Columns

This table contains 10 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [FaecherThemen](../../tables/faecherthemen)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Schluessel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Statistikschlüssel

**`FUBezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Thema`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [FaecherThemen](../../tables/faecherthemen)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

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

**`FaecherUnterpunkte`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_FAECHERUNTERPUNKTE_THEMA`**

:   `Mandant, Thema` » [`FaecherThemen (ID, Mandant)`](../../tables/faecherthemen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_FAECHERUNTERPUNKTE_MANDANTEN`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 6 indices.

**`FK_FAECHERUNTERPUNKTE_MANDANTEN`**

:   `Mandant`

**`FK_FAECHERUNTERPUNKTE_THEMA`**

:   `Mandant, Thema`

**`IDX_FaecherUnterpunkte_Kuerzel`**

:   `Kuerzel`

**`IDX_FaecherUnterpunkte_Mandant`**

:   `Mandant`

**`IDX_FaecherUnterpunkte_Thema`**

:   `Mandant, Thema`

**`PK_FaecherUnterpunkte`**

:   `Mandant, ID`
