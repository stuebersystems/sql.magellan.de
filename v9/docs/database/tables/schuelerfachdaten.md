# Tabelle **SchuelerFachdaten**

## Spalten

Diese Tabelle hat 49 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

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

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`GUIDExtern`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Fachstatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachstati](../../tables/fachstati)

**`Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`Schwerpunkt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachschwerpunkte](../../tables/fachschwerpunkte)

**`Niveau`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [FachNiveaus](../../tables/fachniveaus)

**`KursNr`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Thema`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Beurteilung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Note1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note3`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note4`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note5`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note6`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note7`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note8`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note9`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note10`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note11`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note12`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note13`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Note14`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Vornote`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Endnote1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Endnote2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`Faktor`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`ZusatzKlasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`IstStammkurs`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Endnote1Fortschreiben`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Mahnung`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Mahnung
    1 | Nachmahnung
    2 | Nachprüfung

**`Hauptfach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HausaufgabenVergessen`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`ArbeitsmittelVergessen`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Leistungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Leistungsarten](../../tables/leistungsarten)

**`Durchschnitt`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Bestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    P | Bestanden
    F | Nicht bestanden
    N | Nicht belegt

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerFachdaten`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 27 Fremdschlüssel.

**`FK_SCHUELERFACHDATEN_EN1`**

:   `Endnote1, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_EN2`**

:   `Endnote2, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_FACH`**

:   `Fach, Mandant` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_FACHSTATUS`**

:   `Fachstatus` » [`Fachstati (Kuerzel)`](../../tables/fachstati) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_HAUPTFACH`**

:   `Hauptfach, Mandant` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELERFACHDATEN_LART`**

:   `Leistungsart` » [`Leistungsarten (Kuerzel)`](../../tables/leistungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERFACHDATEN_LEHRER`**

:   `Lehrer, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NIVEAU`**

:   `Niveau` » [`FachNiveaus (Kuerzel)`](../../tables/fachniveaus) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERFACHDATEN_NOTE1`**

:   `Mandant, Note1` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE10`**

:   `Mandant, Note10` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE11`**

:   `Mandant, Note11` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE12`**

:   `Mandant, Note12` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE13`**

:   `Mandant, Note13` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE14`**

:   `Mandant, Note14` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE2`**

:   `Mandant, Note2` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE3`**

:   `Mandant, Note3` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE4`**

:   `Mandant, Note4` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE5`**

:   `Mandant, Note5` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE6`**

:   `Mandant, Note6` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE7`**

:   `Mandant, Note7` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE8`**

:   `Mandant, Note8` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_NOTE9`**

:   `Mandant, Note9` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_SCHWERPKT`**

:   `Schwerpunkt` » [`Fachschwerpunkte (Kuerzel)`](../../tables/fachschwerpunkte) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_TERM`**

:   `Mandant, SchuelerZeitraumID` » [`SchuelerZeitraeume (ID, Mandant)`](../../tables/schuelerzeitraeume) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERFACHDATEN_UNTERRICHT`**

:   `Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_VORNOTE`**

:   `Mandant, Vornote` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERFACHDATEN_ZUSKLASSE`**

:   `Mandant, ZusatzKlasse` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

## Indizes

Diese Tabelle hat 29 Indizes.

**`FK_SCHUELERFACHDATEN_BILING`**

:   `Bilingual`

**`FK_SCHUELERFACHDATEN_EN1`**

:   `Mandant, Endnote1`

**`FK_SCHUELERFACHDATEN_EN2`**

:   `Mandant, Endnote2`

**`FK_SCHUELERFACHDATEN_FACH`**

:   `Mandant, Fach`

**`FK_SCHUELERFACHDATEN_FACHSTATUS`**

:   `Fachstatus`

**`FK_SCHUELERFACHDATEN_HAUPTFACH`**

:   `Mandant, Hauptfach`

**`FK_SCHUELERFACHDATEN_LART`**

:   `Leistungsart`

**`FK_SCHUELERFACHDATEN_LEHRER`**

:   `Mandant, Lehrer`

**`FK_SCHUELERFACHDATEN_NIVEAU`**

:   `Niveau`

**`FK_SCHUELERFACHDATEN_NOTE1`**

:   `Mandant, Note1`

**`FK_SCHUELERFACHDATEN_NOTE10`**

:   `Mandant, Note10`

**`FK_SCHUELERFACHDATEN_NOTE11`**

:   `Mandant, Note11`

**`FK_SCHUELERFACHDATEN_NOTE12`**

:   `Mandant, Note12`

**`FK_SCHUELERFACHDATEN_NOTE13`**

:   `Mandant, Note13`

**`FK_SCHUELERFACHDATEN_NOTE14`**

:   `Mandant, Note14`

**`FK_SCHUELERFACHDATEN_NOTE2`**

:   `Mandant, Note2`

**`FK_SCHUELERFACHDATEN_NOTE3`**

:   `Mandant, Note3`

**`FK_SCHUELERFACHDATEN_NOTE4`**

:   `Mandant, Note4`

**`FK_SCHUELERFACHDATEN_NOTE5`**

:   `Mandant, Note5`

**`FK_SCHUELERFACHDATEN_NOTE6`**

:   `Mandant, Note6`

**`FK_SCHUELERFACHDATEN_NOTE7`**

:   `Mandant, Note7`

**`FK_SCHUELERFACHDATEN_NOTE8`**

:   `Mandant, Note8`

**`FK_SCHUELERFACHDATEN_NOTE9`**

:   `Mandant, Note9`

**`FK_SCHUELERFACHDATEN_SCHWERPKT`**

:   `Schwerpunkt`

**`FK_SCHUELERFACHDATEN_TERM`**

:   `Mandant, SchuelerZeitraumID`

**`FK_SCHUELERFACHDATEN_UNTERRICHT`**

:   `Unterrichtsart`

**`FK_SCHUELERFACHDATEN_VORNOTE`**

:   `Mandant, Vornote`

**`FK_SCHUELERFACHDATEN_ZUSKLASSE`**

:   `Mandant, ZusatzKlasse`

**`PK_SCHUELERFACHDATEN`**

:   `Mandant, ID`
