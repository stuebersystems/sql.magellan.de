# Tabelle **KlassenZeitraeume**

## Spalten

Diese Tabelle hat 19 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Sorgeberechtigte](../../tables/sorgeberechtigte)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`GUIDExtern`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Jahrgang`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Klassenleiter1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Klassenleiter2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Klassenstufe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Klassenstufen](../../tables/klassenstufen)

**`Fachtafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachtafeln](../../tables/fachtafeln)

**`Unterrichtsform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsformen](../../tables/unterrichtsformen)

**`Unterrichtstage`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Klassensprecher1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Klassensprecher2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Klassenelternsprecher1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Sorgeberechtigte](../../tables/sorgeberechtigte)

**`Klassenelternsprecher2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Sorgeberechtigte](../../tables/sorgeberechtigte)

**`Klassenwahlvertreter1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Sorgeberechtigte](../../tables/sorgeberechtigte)

**`Klassenwahlvertreter2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Sorgeberechtigte](../../tables/sorgeberechtigte)

**`Klassenraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Raeume](../../tables/raeume)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`KlassenZeitraeume`**

:   `Mandant, Klasse, Zeitraum`

## Fremdschlüssel

Diese Tabelle hat 13 Fremdschlüssel.

**`FK_KLASSENZEITRAEUME_ELTERN2`**

:   `Klassenelternsprecher2, Mandant` » [`Sorgeberechtigte (ID, Mandant)`](../../tables/sorgeberechtigte) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_FACHTAFEL`**

:   `Fachtafel, Mandant` » [`Fachtafeln (Kuerzel, Mandant)`](../../tables/fachtafeln) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_KLASSE`**

:   `Klasse, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_KLASSENZEITRAEUME_LEITER1`**

:   `Klassenleiter1, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_LEITER2`**

:   `Klassenleiter2, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_RAUM`**

:   `Klassenraum, Mandant` » [`Raeume (ID, Mandant)`](../../tables/raeume) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_SPRECHER1`**

:   `Klassensprecher1, Mandant` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_SPRECHER2`**

:   `Klassensprecher2, Mandant` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_STUFE`**

:   `Klassenstufe` » [`Klassenstufen (Kuerzel)`](../../tables/klassenstufen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSENZEITRAEUME_UNTERRICHT`**

:   `Unterrichtsform` » [`Unterrichtsformen (Kuerzel)`](../../tables/unterrichtsformen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSENZEITRAEUME_WAHL1`**

:   `Klassenwahlvertreter1, Mandant` » [`Sorgeberechtigte (ID, Mandant)`](../../tables/sorgeberechtigte) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_WAHL2`**

:   `Klassenwahlvertreter2, Mandant` » [`Sorgeberechtigte (ID, Mandant)`](../../tables/sorgeberechtigte) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSENZEITRAEUME_ZEITRAUM`**

:   `Zeitraum` » [`Zeitraeume (ID)`](../../tables/zeitraeume) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

## Indizes

Diese Tabelle hat 16 Indizes.

**`FK_KLASSENZEITRAEUME_ELTERN1`**

:   `Mandant, Klassenelternsprecher1`

**`FK_KLASSENZEITRAEUME_ELTERN2`**

:   `Mandant, Klassenelternsprecher2`

**`FK_KLASSENZEITRAEUME_FACHTAFEL`**

:   `Mandant, Fachtafel`

**`FK_KLASSENZEITRAEUME_KLASSE`**

:   `Mandant, Klasse`

**`FK_KLASSENZEITRAEUME_LEITER1`**

:   `Mandant, Klassenleiter1`

**`FK_KLASSENZEITRAEUME_LEITER2`**

:   `Mandant, Klassenleiter2`

**`FK_KLASSENZEITRAEUME_RAUM`**

:   `Mandant, Klassenraum`

**`FK_KLASSENZEITRAEUME_SPRECHER1`**

:   `Mandant, Klassensprecher1`

**`FK_KLASSENZEITRAEUME_SPRECHER2`**

:   `Mandant, Klassensprecher2`

**`FK_KLASSENZEITRAEUME_STUFE`**

:   `Klassenstufe`

**`FK_KLASSENZEITRAEUME_UNTERRICHT`**

:   `Unterrichtsform`

**`FK_KLASSENZEITRAEUME_WAHL1`**

:   `Mandant, Klassenwahlvertreter1`

**`FK_KLASSENZEITRAEUME_WAHL2`**

:   `Mandant, Klassenwahlvertreter2`

**`FK_KLASSENZEITRAEUME_ZEITRAUM`**

:   `Zeitraum`

**`PK2_KLASSENZEITRAEUME`**

:   `Mandant, ID`

**`PK_KLASSENZEITRAEUME`**

:   `Mandant, Klasse, Zeitraum`
