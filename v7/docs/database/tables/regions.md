# Table **Regions**

## Columns

This table contains 12 columns.

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Parent`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Schluessel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Statistikschlüssel

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung

**`Land`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Staaten](../../tables/staaten)

**`RegionTyp`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [RegionTypes](../../tables/regiontypes)

**`StatistikID`**

:   [`VARCHAR(16)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`InternalCode`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Interner Code\. Mögliche Werte werden zukünftig noch festgelegt

**`GueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig ab

**`GueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig bis

## Primary key

This table has a primary key.

**`Regions`**

:   `ID`

## Foreign keys

This table has one foreign key.

**`FK_REGIONS_STAAT`**

:   `Land` » [`Staaten (ID)`](../../tables/staaten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_REGIONS_TYPE`**

:   `RegionTyp` » [`RegionTypes (ID)`](../../tables/regiontypes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indices

This table has 4 indices.

**`FK_REGIONS_PARENT`**

:   `Parent`

**`FK_REGIONS_STAAT`**

:   `Land`

**`FK_REGIONS_TYPE`**

:   `RegionTyp`

**`PK_REGIONS`**

:   `ID`
