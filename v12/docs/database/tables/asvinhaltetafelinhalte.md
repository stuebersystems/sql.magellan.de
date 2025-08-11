# Tabelle **ASVInhaltetafelInhalte**

## Spalten

Diese Tabelle hat 6 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`ASVInhaltetafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [ASVInhaltetafeln](../../tables/asvinhaltetafeln)

**`Schwerpunkt`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes) · `NOT NULL`

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`ASVInhaltetafelInhalte`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_ASVINTAFELIN_INHALTETAFEL`**

:   `ASVInhaltetafel, Mandant` » [`ASVInhaltetafeln (Kuerzel, Mandant)`](../../tables/asvinhaltetafeln) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 2 Indizes.

**`FK_ASVINTAFELIN_INHALTETAFEL`**

:   `Mandant, ASVInhaltetafel`

**`PK_ASVINHALTETAFELINHALTE`**

:   `Mandant, ID`
