# Tabelle **Schuelergruppen**

## Spalten

Diese Tabelle hat 6 Spalten.

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

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Schuelergruppen`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_SGRUPPEN_UEINHEITLEHR`**

:   `Mandant, UnterrichtseinheitLehrer` » [`UnterrichtseinheitenLehrer (ID, Mandant)`](../../tables/unterrichtseinheitenlehrer) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 2 Indizes.

**`FK_SGRUPPEN_UEINHEITLEHR`**

:   `Mandant, UnterrichtseinheitLehrer`

**`PK_SGRUPPEN`**

:   `Mandant, ID`
