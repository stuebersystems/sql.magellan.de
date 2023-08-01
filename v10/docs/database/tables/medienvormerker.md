# Table **MedienVormerker**

## Columns

This table contains 6 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Medium`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Medien](../../tables/medien)

**`Ausleiher`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [MedienAusleiher](../../tables/medienausleiher)

**`VorgemerktAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`VorgemerktUm`**

:   [`TIME`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

## Primary key

This table has a primary key.

**`MedienVormerker`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_MEDIENVORMERKER_MEDIUM`**

:   `Mandant, Medium` » [`Medien (ID, Mandant)`](../../tables/medien) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 4 indices.

**`FK_MEDIENVORMERKER_MEDIUM`**

:   `Mandant, Medium`

**`IDX_MVM_AUSLEIHER`**

:   `Mandant, Ausleiher`

**`IDX_MVM_MEDIUM`**

:   `Mandant, Medium`

**`PK_MEDIENVORMERKER`**

:   `Mandant, ID`
