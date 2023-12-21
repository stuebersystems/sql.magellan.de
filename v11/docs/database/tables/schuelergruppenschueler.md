# Tabelle **SchuelergruppenSchueler**

## Spalten

Diese Tabelle hat 5 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Schuelergruppe`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`Zugang`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Abgang`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelergruppenSchueler`**

:   `Mandant, Schueler, Schuelergruppe`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_SGRUPPENSCHUELER_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SGRUPPENSCHUELER_GRUPPE`**

:   `Mandant, Schuelergruppe` » [`Schuelergruppen (ID, Mandant)`](../../tables/schuelergruppen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_SGRUPPENSCHUELER_GRUPPE`**

:   `Mandant, Schuelergruppe`

**`FK_SGRUPPENSCHUELER_SCHUELER`**

:   `Mandant, Schueler`

**`PK_SGRUPPENSCHUELER`**

:   `Mandant, Schueler, Schuelergruppe`
