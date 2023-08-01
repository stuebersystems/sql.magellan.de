# Table **Schuelergruppen**

## Columns

This table contains 6 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`UnterrichtseinheitLehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`Kuerzel`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

**`Langname1`**

:   [`VARCHAR(150)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Langname2`**

:   [`VARCHAR(150)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primary key

This table has a primary key.

**`Schuelergruppen`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_SGRUPPEN_UEINHEITLEHR`**

:   `Mandant, UnterrichtseinheitLehrer` » [`UnterrichtseinheitenLehrer (ID, Mandant)`](../../tables/unterrichtseinheitenlehrer) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 2 indices.

**`FK_SGRUPPEN_UEINHEITLEHR`**

:   `Mandant, UnterrichtseinheitLehrer`

**`PK_SGRUPPEN`**

:   `Mandant, ID`
