# Table **SchuelerKlassen**

## Columns

This table contains 33 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerZeitraeume](../../tables/schuelerzeitraeume)

**`Hauptklasse`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Zugang`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Abgang`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Wiederholer`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Wiederholungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Wiederholungsarten](../../tables/wiederholungsarten)

**`Ueberspringer`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Versetzt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Versetzungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Versetzungsarten](../../tables/versetzungsarten)

**`VersetztAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`SchulformEintritt`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Fachtafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachtafeln](../../tables/fachtafeln)

**`Aufnahmepruefung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Aufnahmepruefungen](../../tables/aufnahmepruefungen)

**`AufnahmepruefungBestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Nachpruefung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Nachpruefungen](../../tables/nachpruefungen)

**`NachpruefungBestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Empfehlung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Empfehlungen](../../tables/empfehlungen)

**`Elternwunsch`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Empfehlungen](../../tables/empfehlungen)

**`Verordnung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Verordnungen](../../tables/verordnungen)

**`Meldungen`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Abschluss1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Abschluss1Art`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abschlussarten](../../tables/abschlussarten)

**`Abschluss1Datum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Abschluss1Note`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Abschluss2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [AbschluesseIntern](../../tables/abschluesseintern)

**`Abschluss2Art`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abschlussarten](../../tables/abschlussarten)

**`Abschluss2Datum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Abschluss2Note`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`KlassenzielErreicht`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`KlassenzielErreichtAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Entscheidung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Entscheidungen](../../tables/entscheidungen)

**`Schulart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schularten](../../tables/schularten)

## Primary key

This table has a primary key.

**`SchuelerKlassen`**

:   `Mandant, SchuelerZeitraumID`

## Foreign keys

This table has one foreign key.

**`FK_SCHUELERKLASSEN_ABSCHLUSS1A`**

:   `Abschluss1Art` » [`Abschlussarten (Kuerzel)`](../../tables/abschlussarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_ABSCHLUSS2`**

:   `Abschluss2` » [`AbschluesseIntern (Kuerzel)`](../../tables/abschluesseintern) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_ABSCHLUSS2A`**

:   `Abschluss2Art` » [`Abschlussarten (Kuerzel)`](../../tables/abschlussarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_AUFNAHME`**

:   `Aufnahmepruefung` » [`Aufnahmepruefungen (Kuerzel)`](../../tables/aufnahmepruefungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_ELTERNWUNSCH`**

:   `Elternwunsch` » [`Empfehlungen (Kuerzel)`](../../tables/empfehlungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_EMPFEHLUNG`**

:   `Empfehlung` » [`Empfehlungen (Kuerzel)`](../../tables/empfehlungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_ENTSCHEIDUNG`**

:   `Entscheidung` » [`Entscheidungen (Kuerzel)`](../../tables/entscheidungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_FACHTAFEL`**

:   `Fachtafel, Mandant` » [`Fachtafeln (Kuerzel, Mandant)`](../../tables/fachtafeln) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERKLASSEN_NACHPRUEF`**

:   `Nachpruefung` » [`Nachpruefungen (Kuerzel)`](../../tables/nachpruefungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_SCHULART`**

:   `Schulart` » [`Schularten (Kuerzel)`](../../tables/schularten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_STUDENTTERM`**

:   `Mandant, SchuelerZeitraumID` » [`SchuelerZeitraeume (ID, Mandant)`](../../tables/schuelerzeitraeume) · `ON UPDATE NO ACTION` · `ON DELETE CASCADE`

**`FK_SCHUELERKLASSEN_VERORDNUNG`**

:   `Verordnung` » [`Verordnungen (Kuerzel)`](../../tables/verordnungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_VERSETZUNG`**

:   `Versetzungsart` » [`Versetzungsarten (Kuerzel)`](../../tables/versetzungsarten) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERKLASSEN_WIEDERHOLUNG`**

:   `Wiederholungsart` » [`Wiederholungsarten (Kuerzel)`](../../tables/wiederholungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERKLASSEN_ABSCHLUSS1`**

:   `Abschluss1` » [`AbschluesseIntern (Kuerzel)`](../../tables/abschluesseintern) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indices

This table has 16 indices.

**`FK_SCHUELERKLASSEN_ABSCHLUSS1`**

:   `Abschluss1`

**`FK_SCHUELERKLASSEN_ABSCHLUSS1A`**

:   `Abschluss1Art`

**`FK_SCHUELERKLASSEN_ABSCHLUSS2`**

:   `Abschluss2`

**`FK_SCHUELERKLASSEN_ABSCHLUSS2A`**

:   `Abschluss2Art`

**`FK_SCHUELERKLASSEN_AUFNAHME`**

:   `Aufnahmepruefung`

**`FK_SCHUELERKLASSEN_ELTERNWUNSCH`**

:   `Elternwunsch`

**`FK_SCHUELERKLASSEN_EMPFEHLUNG`**

:   `Empfehlung`

**`FK_SCHUELERKLASSEN_ENTSCHEIDUNG`**

:   `Entscheidung`

**`FK_SCHUELERKLASSEN_FACHTAFEL`**

:   `Mandant, Fachtafel`

**`FK_SCHUELERKLASSEN_NACHPRUEF`**

:   `Nachpruefung`

**`FK_SCHUELERKLASSEN_SCHULART`**

:   `Schulart`

**`FK_SCHUELERKLASSEN_STUDENTTERM`**

:   `Mandant, SchuelerZeitraumID`

**`FK_SCHUELERKLASSEN_VERORDNUNG`**

:   `Verordnung`

**`FK_SCHUELERKLASSEN_VERSETZUNG`**

:   `Versetzungsart`

**`FK_SCHUELERKLASSEN_WIEDERHOLUNG`**

:   `Wiederholungsart`

**`PK_SCHUELERKLASSEN`**

:   `Mandant, SchuelerZeitraumID`
