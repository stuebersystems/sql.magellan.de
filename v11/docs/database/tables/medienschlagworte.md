# Tabelle **MedienSchlagworte**

## Spalten

Diese Tabelle hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schlagworte](../../tables/schlagworte)

**`Medium`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Medien](../../tables/medien)

**`Schlagwort`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schlagworte](../../tables/schlagworte)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`MedienSchlagworte`**

:   `Mandant, Medium, Schlagwort`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_MEDIENSCHLAGWORTE_SCHLAGWORT`**

:   `Mandant, Schlagwort` » [`Schlagworte (ID, Mandant)`](../../tables/schlagworte) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_MEDIENSCHLAGWORTE_MEDIUM`**

:   `Mandant, Medium` » [`Medien (ID, Mandant)`](../../tables/medien) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_MEDIENSCHLAGWORTE_MEDIUM`**

:   `Mandant, Medium`

**`FK_MEDIENSCHLAGWORTE_SCHLAGWORT`**

:   `Mandant, Schlagwort`

**`PK_MEDIENSCHLAGWORTE`**

:   `Mandant, Medium, Schlagwort`
