# Table **UnterrichtseinheitenLehrer**

## Columns

This table contains 7 columns.

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

    Iststunden \(=Lehrer\-Ist aus DAVINCI\)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Gruppenunterricht`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Ist nur Unterricht in einer Schülergruppe?

    Value | Description
    - | -
    N | Nein
    J | Ja

## Primary key

This table has a primary key.

**`UnterrichtseinheitenLehrer`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_UEINHEITENLEHRER_UEINHEIT`**

:   `Mandant, Unterrichtseinheit` » [`Unterrichtseinheiten (ID, Mandant)`](../../tables/unterrichtseinheiten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_UEINHEITENLEHRER_LEHRER`**

:   `Lehrer, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

## Indices

This table has 3 indices.

**`FK_UEINHEITENLEHRER_LEHRER`**

:   `Mandant, Lehrer`

**`FK_UEINHEITENLEHRER_UEINHEIT`**

:   `Mandant, Unterrichtseinheit`

**`PK_UEINHEITENLEHRER`**

:   `Mandant, ID`
