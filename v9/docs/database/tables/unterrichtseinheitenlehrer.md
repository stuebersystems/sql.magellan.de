# Tabelle **UnterrichtseinheitenLehrer**

## Spalten

Diese Tabelle hat 7 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Unterrichtseinheiten](../../tables/unterrichtseinheiten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Unterrichtseinheit`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Unterrichtseinheiten](../../tables/unterrichtseinheiten)

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Ist`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Iststunden \(=Lehrer\-Ist aus DaVinci\)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Gruppenunterricht`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Ist nur Unterricht in einer Schülergruppe?

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`UnterrichtseinheitenLehrer`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_UEINHEITENLEHRER_UEINHEIT`**

:   `Mandant, Unterrichtseinheit` » [`Unterrichtseinheiten (ID, Mandant)`](../../tables/unterrichtseinheiten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_UEINHEITENLEHRER_LEHRER`**

:   `Mandant, Lehrer`

**`FK_UEINHEITENLEHRER_UEINHEIT`**

:   `Mandant, Unterrichtseinheit`

**`PK_UEINHEITENLEHRER`**

:   `Mandant, ID`
