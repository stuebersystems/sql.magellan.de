# Table **SchulenKontakte**

## Columns

This table contains 4 columns.

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Eindeutige ID

**`Schule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Kontakt`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`KontaktInfo`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primary key

This table has a primary key.

**`SchulenKontakte`**

:   `ID`

## Foreign keys

This table has one foreign key.

**`FK_SCHULENKT_SCHULE`**

:   `Schule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 2 indices.

**`FK_SCHULENKT_SCHULE`**

:   `Schule`

**`PK_SCHULENKONTAKTE`**

:   `ID`
