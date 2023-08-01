# Tabelle **AdressenKontakte**

## Spalten

Diese Tabelle hat 5 Spalten.

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

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`AdressenKontakte`**

:   `Mandant, ID`

## Indizes

Diese Tabelle hat 4 Indizes.

**`FK_ADRESSENKT_ADRESSE`**

:   `Mandant, Adresse`

**`IDX_AdressenKontakte_Adresse`**

:   `Mandant, Adresse`

**`IDX_AdressenKontakte_ID`**

:   `ID, Mandant`

**`PK_ADRESSENKONTAKTE`**

:   `Mandant, ID`
