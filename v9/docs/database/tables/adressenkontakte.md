# Table **AdressenKontakte**

## Columns

This table contains 5 columns.

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Adresse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Adressen](../../tables/adressen)

**`Kontakt`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`KontaktInfo`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primary key

This table has a primary key.

**`AdressenKontakte`**

:   `Mandant, ID`

## Indices

This table has 4 indices.

**`FK_ADRESSENKT_ADRESSE`**

:   `Mandant, Adresse`

**`IDX_AdressenKontakte_Adresse`**

:   `Mandant, Adresse`

**`IDX_AdressenKontakte_ID`**

:   `ID, Mandant`

**`PK_ADRESSENKONTAKTE`**

:   `Mandant, ID`
