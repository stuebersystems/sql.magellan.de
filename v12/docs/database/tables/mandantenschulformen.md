# Tabelle **MandantenSchulformen**

## Spalten

Diese Tabelle hat 4 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Schulformen](../../tables/schulformen)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`MandantenSchulformen`**

:   `Mandant, Schulform`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_MANDANTENSCHULFORMEN_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_MANDANTENSCHULFORMEN_FORM`**

:   `Schulform` » [`Schulformen (Kuerzel)`](../../tables/schulformen) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_MANDANTENSCHULFORMEN_FORM`**

:   `Schulform`

**`FK_MANDANTENSCHULFORMEN_MANDANT`**

:   `Mandant`

**`PK_MANDANTENSCHULFORMEN`**

:   `Mandant, Schulform`
