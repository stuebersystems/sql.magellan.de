# Table **PersonenMedizinDaten**

## Columns

This table contains 11 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [MedizinKategorien](../../tables/medizinkategorien)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Person`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Personen](../../tables/personen)

**`Kategorie`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [MedizinKategorien](../../tables/medizinkategorien)

**`Art`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [MedizinArten](../../tables/medizinarten)

**`Medikamente`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Medikationen`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Bemerkung1`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Bemerkung2`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`AblaufAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

## Primary key

This table has a primary key.

**`PersonenMedizinDaten`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_PERSONENMEDIZINDATEN_ART`**

:   `Art, Mandant` » [`MedizinArten (ID, Mandant)`](../../tables/medizinarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_PERSONENMEDIZINDATEN_KAT`**

:   `Kategorie, Mandant` » [`MedizinKategorien (ID, Mandant)`](../../tables/medizinkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indices

This table has 4 indices.

**`FK_PERSONENMEDDAT_PERSON`**

:   `Mandant, Person`

**`FK_PERSONENMEDIZINDATEN_ART`**

:   `Mandant, Art`

**`FK_PERSONENMEDIZINDATEN_KAT`**

:   `Mandant, Kategorie`

**`PK_PERSONENMEDIZINDATEN`**

:   `Mandant, ID`
