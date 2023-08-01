# Table **MedienSchlagworte**

## Columns

This table contains 3 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schlagworte](../../tables/schlagworte)

**`Medium`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Medien](../../tables/medien)

**`Schlagwort`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schlagworte](../../tables/schlagworte)

## Primary key

This table has a primary key.

**`MedienSchlagworte`**

:   `Mandant, Medium, Schlagwort`

## Foreign keys

This table has one foreign key.

**`FK_MEDIENSCHLAGWORTE_SCHLAGWORT`**

:   `Mandant, Schlagwort` » [`Schlagworte (ID, Mandant)`](../../tables/schlagworte) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_MEDIENSCHLAGWORTE_MEDIUM`**

:   `Mandant, Medium` » [`Medien (ID, Mandant)`](../../tables/medien) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_MEDIENSCHLAGWORTE_MEDIUM`**

:   `Mandant, Medium`

**`FK_MEDIENSCHLAGWORTE_SCHLAGWORT`**

:   `Mandant, Schlagwort`

**`PK_MEDIENSCHLAGWORTE`**

:   `Mandant, Medium, Schlagwort`
