# Table **SchuelerBBSZeugnisformulare**

## Columns

This table contains 5 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`Formular`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Zeugnisformulare](../../tables/zeugnisformulare)

## Primary key

This table has a primary key.

**`SchuelerBBSZeugnisformulare`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_SCHUELERBBSZ_FORMULAR`**

:   `Formular, Mandant` » [`Zeugnisformulare (ID, Mandant)`](../../tables/zeugnisformulare) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERBBSZ_SCHUELERZEITR`**

:   `Mandant, SchuelerZeitraumID` » [`SchuelerZeitraeume (ID, Mandant)`](../../tables/schuelerzeitraeume) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 4 indices.

**`FK_SCHUELERBBSZ_BBS`**

:   `Mandant, Schueler`

**`FK_SCHUELERBBSZ_FORMULAR`**

:   `Mandant, Formular`

**`FK_SCHUELERBBSZ_SCHUELERZEITR`**

:   `Mandant, SchuelerZeitraumID`

**`PK_SCHUELERBBSFORMULARE`**

:   `Mandant, ID`
