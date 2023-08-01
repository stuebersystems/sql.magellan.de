# Tabelle **ASVTafelKategorien**

## Spalten

Diese Tabelle hat 7 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [ASVInhaltetafeln](../../tables/asvinhaltetafeln)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`ASVTafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [ASVTafeln](../../tables/asvtafeln)

**`Kategorie`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [ASVKategorien](../../tables/asvkategorien)

**`ASVInhaltetafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [ASVInhaltetafeln](../../tables/asvinhaltetafeln)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`ASVTafelKategorien`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_ASVTAFELKATEGORIEN_KATEGORIE`**

:   `Kategorie` » [`ASVKategorien (Kuerzel)`](../../tables/asvkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_ASVTAFELKAT_INHALTETAFEL`**

:   `ASVInhaltetafel, Mandant` » [`ASVInhaltetafeln (Kuerzel, Mandant)`](../../tables/asvinhaltetafeln) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 4 Indizes.

**`FK_ASVTAFELKATEGORIEN_ASVTAFEL`**

:   `Mandant, ASVTafel`

**`FK_ASVTAFELKATEGORIEN_KATEGORIE`**

:   `Kategorie`

**`FK_ASVTAFELKAT_INHALTETAFEL`**

:   `Mandant, ASVInhaltetafel`

**`PK_ASVTAFELKATEGORIEN`**

:   `Mandant, ID`
