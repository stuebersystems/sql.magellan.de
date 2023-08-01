# Tabelle **SchuelerABIZeugnisformulare**

## Spalten

Diese Tabelle hat 7 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Formular`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Zeugnisformulare](../../tables/zeugnisformulare)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerABIZeugnisformulare`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 3 Fremdschlüssel.

**`FK_SCHUELERABIZ_FORMULAR`**

:   `Formular, Mandant` » [`Zeugnisformulare (ID, Mandant)`](../../tables/zeugnisformulare) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERABIZ_SCHUELERZEITR`**

:   `Mandant, SchuelerZeitraumID` » [`SchuelerZeitraeume (ID, Mandant)`](../../tables/schuelerzeitraeume) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERABIZ_ABI`**

:   `Mandant, Schueler` » [`SchuelerABI (Mandant, Schueler)`](../../tables/schuelerabi) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 4 Indizes.

**`FK_SCHUELERABIZ_ABI`**

:   `Mandant, Schueler`

**`FK_SCHUELERABIZ_FORMULAR`**

:   `Mandant, Formular`

**`FK_SCHUELERABIZ_SCHUELERZEITR`**

:   `Mandant, SchuelerZeitraumID`

**`PK_SCHUELERABIFORMULARE`**

:   `Mandant, ID`
