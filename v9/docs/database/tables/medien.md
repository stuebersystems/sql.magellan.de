# Table **Medien**

## Columns

This table contains 37 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Standorte](../../tables/standorte)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Barcode`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BarcodePrint`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`InventarNr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Titel`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Untertitel`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Medienart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Medienarten](../../tables/medienarten)

**`Medienkategorie`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [MedienKategorien](../../tables/medienkategorien)

**`Standort`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Standorte](../../tables/standorte)

**`Verlag`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Verlage](../../tables/verlage)

**`Verlagsname`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Verlagsort`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Herausgeber`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Autor`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Signaturvorgabe`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Copyright`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`ISBN`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`ISSN`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Erscheinungsjahr`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Erscheinungsland`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Staaten](../../tables/staaten)

**`Erscheinungsweise`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Erscheinungsweisen](../../tables/erscheinungsweisen)

**`Sprache`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Sprachen](../../tables/sprachen)

**`Format`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Medienformate](../../tables/medienformate)

**`Umfang`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Serie`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Band`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Heft`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Ausgabe`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Jahrgang`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Zusammenfassung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Ausleihbar
    1 | Nicht ausleihbar
    2 | Nicht aktuell
    3 | Dauerverleih \/ Teilweise Dauerverleih
    4 |  Dauerleihgabe \/ Teilweise Dauerleihgabe

**`Mehrjahresband`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Value | Description
    - | -
    N | Nein
    J | Ja

**`JahrgangVon`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [MedienJahrgaenge](../../tables/medienjahrgaenge)

**`JahrgangBis`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [MedienJahrgaenge](../../tables/medienjahrgaenge)

## Primary key

This table has a primary key.

**`Medien`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_MEDIEN_ERSCHEINUNGSWEISE`**

:   `Erscheinungsweise` » [`Erscheinungsweisen (Kuerzel)`](../../tables/erscheinungsweisen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_MEDIEN_FORMAT`**

:   `Format` » [`Medienformate (Kuerzel)`](../../tables/medienformate) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_MEDIEN_JAHRGANGBIS`**

:   `JahrgangBis` » [`MedienJahrgaenge (Kuerzel)`](../../tables/medienjahrgaenge) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_MEDIEN_JAHRGANGVON`**

:   `JahrgangVon` » [`MedienJahrgaenge (Kuerzel)`](../../tables/medienjahrgaenge) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_MEDIEN_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_MEDIEN_MEDIENART`**

:   `Medienart` » [`Medienarten (Kuerzel)`](../../tables/medienarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_MEDIEN_MEDIENKATEGORIE`**

:   `Medienkategorie` » [`MedienKategorien (Kuerzel)`](../../tables/medienkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_MEDIEN_SPRACHE`**

:   `Sprache` » [`Sprachen (Kuerzel)`](../../tables/sprachen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_MEDIEN_STANDORT`**

:   `Mandant, Standort` » [`Standorte (Kuerzel, Mandant)`](../../tables/standorte) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_MEDIEN_VERLAG`**

:   `Verlag` » [`Verlage (ID)`](../../tables/verlage) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

## Indices

This table has 13 indices.

**`FK_MEDIEN_ERSCHEINUNGSLAND`**

:   `Erscheinungsland`

**`FK_MEDIEN_ERSCHEINUNGSWEISE`**

:   `Erscheinungsweise`

**`FK_MEDIEN_FORMAT`**

:   `Format`

**`FK_MEDIEN_JAHRGANGBIS`**

:   `JahrgangBis`

**`FK_MEDIEN_JAHRGANGVON`**

:   `JahrgangVon`

**`FK_MEDIEN_MANDANT`**

:   `Mandant`

**`FK_MEDIEN_MEDIENART`**

:   `Medienart`

**`FK_MEDIEN_MEDIENKATEGORIE`**

:   `Medienkategorie`

**`FK_MEDIEN_SPRACHE`**

:   `Sprache`

**`FK_MEDIEN_STANDORT`**

:   `Mandant, Standort`

**`FK_MEDIEN_VERLAG`**

:   `Verlag`

**`IDX_M_SIGNATUR`**

:   `Mandant, Signaturvorgabe`

**`PK_MEDIEN`**

:   `Mandant, ID`
