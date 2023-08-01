# Table **SchuelerASVKategorien**

## Columns

This table contains 10 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Kategorie`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [ASVKategorien](../../tables/asvkategorien)

**`Bewertung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [ASVBewertungen](../../tables/asvbewertungen)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primary key

This table has a primary key.

**`SchuelerASVKategorien`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_SCHUELERASVKATEGORIEN_BEW`**

:   `Bewertung` » [`ASVBewertungen (Kuerzel)`](../../tables/asvbewertungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERASVKATEGORIEN_KAT`**

:   `Kategorie` » [`ASVKategorien (Kuerzel)`](../../tables/asvkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indices

This table has 4 indices.

**`FK_SCHUELERASVKATEGORIEN`**

:   `Mandant, SchuelerZeitraumID`

**`FK_SCHUELERASVKATEGORIEN_BEW`**

:   `Bewertung`

**`FK_SCHUELERASVKATEGORIEN_KAT`**

:   `Kategorie`

**`PK_SCHUELERASVKATEGORIEN`**

:   `Mandant, ID`
