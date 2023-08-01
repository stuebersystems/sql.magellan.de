# Table **WettkampfDisziplinen**

## Columns

This table contains 6 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Wettkaempfe](../../tables/wettkaempfe)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Wettkampf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Wettkaempfe](../../tables/wettkaempfe)

**`Disziplin`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Disziplinen](../../tables/disziplinen)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Freies Merkmal

## Primary key

This table has a primary key.

**`WettkampfDisziplinen`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_WETTKAEMPFE_WETTKAMPF`**

:   `Mandant, Wettkampf` » [`Wettkaempfe (Kuerzel, Mandant)`](../../tables/wettkaempfe) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_WETTKAEMPFE_DISZIPLIN`**

:   `Disziplin, Mandant` » [`Disziplinen (Kuerzel, Mandant)`](../../tables/disziplinen) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_WETTKAEMPFE_DISZIPLIN`**

:   `Mandant, Disziplin`

**`FK_WETTKAEMPFE_WETTKAMPF`**

:   `Mandant, Wettkampf`

**`PK_WETTKAMPFDISZIPLINEN`**

:   `Mandant, ID`
