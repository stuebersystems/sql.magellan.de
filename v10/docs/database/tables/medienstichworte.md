# Table **MedienStichworte**

## Columns

This table contains 4 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Medium`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Medien](../../tables/medien)

**`Stichwort`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Stichwort

## Primary key

This table has a primary key.

**`MedienStichworte`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_MEDIENSTICHWORTE_MEDIUM`**

:   `Mandant, Medium` » [`Medien (ID, Mandant)`](../../tables/medien) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_MEDIENSTICHWORTE_MEDIUM`**

:   `Mandant, Medium`

**`IDX_MSW_MEDIUM`**

:   `Mandant, Medium`

**`PK_MEDIENSTICHWORTE`**

:   `Mandant, ID`
