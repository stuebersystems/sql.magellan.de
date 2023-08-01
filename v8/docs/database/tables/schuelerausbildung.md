# Table **SchuelerAusbildung**

## Columns

This table contains 24 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`GUID`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Betrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Betriebe](../../tables/betriebe)

**`AusbilderKontakt`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`PraxisBetrieb`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Betriebe](../../tables/betriebe)

**`PraxisKontakt`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [BetriebeKontakte](../../tables/betriebekontakte)

**`Beruf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Berufe](../../tables/berufe)

**`Bildungsgang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bildungsgaenge](../../tables/bildungsgaenge)

**`Organisation`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Organisationen](../../tables/organisationen)

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schulformen](../../tables/schulformen)

**`AusbildungVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`AusbildungBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Ausbildungsdauer`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`PraxisVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`PraxisBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Praxisdauer`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Vertrag`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Vertragsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Vertragsarten](../../tables/vertragsarten)

**`Vertragsnr`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`VertragVorgelegtAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Neuanfaenger`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `DEFAULT 'J'`

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primary key

This table has a primary key.

**`SchuelerAusbildung`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_SCHUELERAB_BERUF`**

:   `Beruf` » [`Berufe (Kuerzel)`](../../tables/berufe) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERAB_BETRIEB`**

:   `Betrieb, Mandant` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERAB_BILDUNGSGANG`**

:   `Bildungsgang` » [`Bildungsgaenge (Kuerzel)`](../../tables/bildungsgaenge) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERAB_ORGANISATION`**

:   `Organisation` » [`Organisationen (Kuerzel)`](../../tables/organisationen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERAB_PRAXISBETRIEB`**

:   `Mandant, PraxisBetrieb` » [`Betriebe (ID, Mandant)`](../../tables/betriebe) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELERAB_PRAXISKONTAKT`**

:   `Mandant, PraxisKontakt` » [`BetriebeKontakte (ID, Mandant)`](../../tables/betriebekontakte) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELERAB_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERAB_SCHULFORM`**

:   `Schulform` » [`Schulformen (Kuerzel)`](../../tables/schulformen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERAB_VERTRAGSART`**

:   `Vertragsart` » [`Vertragsarten (Kuerzel)`](../../tables/vertragsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indices

This table has 11 indices.

**`FK_SCHUELERAB_AUSBILDERKONTAKT`**

:   `Mandant, AusbilderKontakt`

**`FK_SCHUELERAB_BERUF`**

:   `Beruf`

**`FK_SCHUELERAB_BETRIEB`**

:   `Mandant, Betrieb`

**`FK_SCHUELERAB_BILDUNGSGANG`**

:   `Bildungsgang`

**`FK_SCHUELERAB_ORGANISATION`**

:   `Organisation`

**`FK_SCHUELERAB_PRAXISBETRIEB`**

:   `Mandant, PraxisBetrieb`

**`FK_SCHUELERAB_PRAXISKONTAKT`**

:   `Mandant, PraxisKontakt`

**`FK_SCHUELERAB_SCHUELER`**

:   `Mandant, Schueler`

**`FK_SCHUELERAB_SCHULFORM`**

:   `Schulform`

**`FK_SCHUELERAB_VERTRAGSART`**

:   `Vertragsart`

**`PK_SCHUELERAB`**

:   `Mandant, ID`
