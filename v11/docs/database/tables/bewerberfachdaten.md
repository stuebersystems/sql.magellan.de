# Tabelle **BewerberFachdaten**

## Spalten

Diese Tabelle hat 8 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Noten](../../tables/noten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Note`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`JahrgangVon`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`JahrgangBis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Kategorie`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`BewerberFachdaten`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_BEWERBERFACHDATEN_NOTE`**

:   `Mandant, Note` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BEWERBERFACHDATEN_FACH`**

:   `Fach, Mandant` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_BEWERBERFACHDATEN_FACH`**

:   `Mandant, Fach`

**`FK_BEWERBERFACHDATEN_NOTE`**

:   `Mandant, Note`

**`PK_BEWERBERFACHDATEN`**

:   `Mandant, ID`
