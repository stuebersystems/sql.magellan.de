# Tabelle **SchuelerMedizinDaten**

## Spalten

Diese Tabelle hat 11 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [MedizinKategorien](../../tables/medizinkategorien)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

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

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerMedizinDaten`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 3 Fremdschlüssel.

**`FK_SCHUELERMEDIZINDATEN_ART`**

:   `Art, Mandant` » [`MedizinArten (ID, Mandant)`](../../tables/medizinarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERMEDIZINDATEN_KAT`**

:   `Kategorie, Mandant` » [`MedizinKategorien (ID, Mandant)`](../../tables/medizinkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERMEDDAT_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 4 Indizes.

**`FK_SCHUELERMEDDAT_SCHUELER`**

:   `Mandant, Schueler`

**`FK_SCHUELERMEDIZINDATEN_ART`**

:   `Mandant, Art`

**`FK_SCHUELERMEDIZINDATEN_KAT`**

:   `Mandant, Kategorie`

**`PK_SCHUELERMEDIZINDATEN`**

:   `Mandant, ID`
