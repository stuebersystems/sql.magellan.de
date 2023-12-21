# Tabelle **SchulenKontakte**

## Spalten

Diese Tabelle hat 4 Spalten.

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

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchulenKontakte`**

:   `ID`

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_SCHULENKT_SCHULE`**

:   `Schule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 2 Indizes.

**`FK_SCHULENKT_SCHULE`**

:   `Schule`

**`PK_SCHULENKONTAKTE`**

:   `ID`
