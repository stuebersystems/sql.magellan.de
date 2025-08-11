# Tabelle **Wettkaempfe**

## Spalten

Diese Tabelle hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Wettkaempfe`**

:   `Mandant, Kuerzel`

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_WETTKAMPF_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 2 Indizes.

**`FK_WETTKAMPF_MANDANT`**

:   `Mandant`

**`PK_WETTKAEMPFE`**

:   `Mandant, Kuerzel`
