# Tabelle **Klassen**

Speichert die Klassen in Magellan

## Spalten

Diese Tabelle hat 55 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externe ENBREA\-ID

**`GUID`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`IDIntern`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`IDExtern`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`GUIDExtern`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Kuerzel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Kürzel der Klasse

**`KuerzelAlpha`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`KuerzelStatistik`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Statistikkürzel der Klasse

**`Langname1`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Erste Langname der Klasse

**`Langname2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Zweite Langname der Klasse

**`Klassenart`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Klassenart

    Wert | Beschreibung
    - | -
    0 | Standardklasse
    1 | Ganztagsklasse
    2 | Oberstufenjahrgang \(Nur Kurse\)
    3 | Oberstufenjahrgang \(Leistungs\- u\. Grundkurse\)
    4 | Abschlussklasse
    5 | Kombinationsklasse
    6 | Schulkindergarten
    7 | Standardklasse mit Oberstufensynchronisation

**`Notenart`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Notenart

    Wert | Beschreibung
    - | -
    0 | Notenwerte
    1 | Punktwerte
    2 | Beurteilungen

**`Abteilung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abteilungen](../../tables/abteilungen)

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schulformen](../../tables/schulformen)

**`Schulart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schularten](../../tables/schularten)

**`Organisation`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Organisationen](../../tables/organisationen)

**`Behinderung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Behinderungsarten](../../tables/behinderungsarten)

**`FoerderSchwerpunkt1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [FoerderSchwerpunkte](../../tables/foerderschwerpunkte)

**`FoerderSchwerpunkt2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [FoerderSchwerpunkte](../../tables/foerderschwerpunkte)

**`Beruf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Berufe](../../tables/berufe)

**`Bildungsgang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bildungsgaenge](../../tables/bildungsgaenge)

**`Integration`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Integrationsmerkmale](../../tables/integrationsmerkmale)

**`Berufsfeld`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Berufsfelder](../../tables/berufsfelder)

**`Einzelintegration`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Laenderuebergreifend`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Regelbetrag`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`Schulartuebergreifend`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Schulstelle`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schulstellen](../../tables/schulstellen)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`MerkmalA1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalA2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalA3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalA4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalA5`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`Foerderung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Foerderungen](../../tables/foerderungen)

**`MerkmalA6`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalS1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalS2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalS3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalS4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [KlassenMerkmale](../../tables/klassenmerkmale)

**`MerkmalB1`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB2`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB3`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB4`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`KBGueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`KBGueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`KBFuehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`KBBemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Klassenorganisation`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Klassenorganisationen](../../tables/klassenorganisationen)

**`Maske`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Standardmaske der Klasse

**`Schuelerplan`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Soll bei der Anzeige der Stundenplans der Schüler der Klasse der individuelle Schülerplan anstelle des Klassenplan angezeigt werden?

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`NaechsteKlasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`NaechsteKlasseZeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Klassen`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 27 Fremdschlüssel.

**`FK_KLASSEN_BEHINDERUNG`**

:   `Behinderung` » [`Behinderungsarten (Kuerzel)`](../../tables/behinderungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_BERUF`**

:   `Beruf` » [`Berufe (Kuerzel)`](../../tables/berufe) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_BERUFSFELD`**

:   `Berufsfeld` » [`Berufsfelder (Kuerzel)`](../../tables/berufsfelder) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_BILDUNGSGANG`**

:   `Bildungsgang` » [`Bildungsgaenge (Kuerzel)`](../../tables/bildungsgaenge) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_FOERDERUNG`**

:   `Foerderung` » [`Foerderungen (Kuerzel)`](../../tables/foerderungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_INTEGRATION`**

:   `Integration` » [`Integrationsmerkmale (Kuerzel)`](../../tables/integrationsmerkmale) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_KLASSEN_KLORGANISATION`**

:   `Klassenorganisation` » [`Klassenorganisationen (Kuerzel)`](../../tables/klassenorganisationen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALA1`**

:   `Mandant, MerkmalA1` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALA2`**

:   `Mandant, MerkmalA2` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALA3`**

:   `Mandant, MerkmalA3` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALA4`**

:   `Mandant, MerkmalA4` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALA5`**

:   `Mandant, MerkmalA5` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALA6`**

:   `Mandant, MerkmalA6` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALS1`**

:   `Mandant, MerkmalS1` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALS2`**

:   `Mandant, MerkmalS2` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALS3`**

:   `Mandant, MerkmalS3` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_MERKMALS4`**

:   `Mandant, MerkmalS4` » [`KlassenMerkmale (Kuerzel, Mandant)`](../../tables/klassenmerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_KLASSEN_NAECHSTEKLASSE`**

:   `Mandant, NaechsteKlasse` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_KLASSEN_NAECHSTEKLASSEZ`**

:   `NaechsteKlasseZeitraum` » [`Zeitraeume (ID)`](../../tables/zeitraeume) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_KLASSEN_ORGANISATION`**

:   `Organisation` » [`Organisationen (Kuerzel)`](../../tables/organisationen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_SCHULART`**

:   `Schulart` » [`Schularten (Kuerzel)`](../../tables/schularten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_SCHULFORM`**

:   `Schulform` » [`Schulformen (Kuerzel)`](../../tables/schulformen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSEN_SCHULSTELLE`**

:   `Schulstelle` » [`Schulstellen (Kuerzel)`](../../tables/schulstellen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_KLASSE_FOERDERSCHWERP1`**

:   `FoerderSchwerpunkt1` » [`FoerderSchwerpunkte (Kuerzel)`](../../tables/foerderschwerpunkte) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_KLASSE_FOERDERSCHWERP2`**

:   `FoerderSchwerpunkt2` » [`FoerderSchwerpunkte (Kuerzel)`](../../tables/foerderschwerpunkte) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_KLASSEN_ABTEILUNG`**

:   `Abteilung, Mandant` » [`Abteilungen (Kuerzel, Mandant)`](../../tables/abteilungen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

## Indizes

Diese Tabelle hat 28 Indizes.

**`FK_KLASSEN_ABTEILUNG`**

:   `Mandant, Abteilung`

**`FK_KLASSEN_BEHINDERUNG`**

:   `Behinderung`

**`FK_KLASSEN_BERUF`**

:   `Beruf`

**`FK_KLASSEN_BERUFSFELD`**

:   `Berufsfeld`

**`FK_KLASSEN_BILDUNGSGANG`**

:   `Bildungsgang`

**`FK_KLASSEN_FOERDERUNG`**

:   `Foerderung`

**`FK_KLASSEN_INTEGRATION`**

:   `Integration`

**`FK_KLASSEN_KLORGANISATION`**

:   `Klassenorganisation`

**`FK_KLASSEN_MANDANT`**

:   `Mandant`

**`FK_KLASSEN_MERKMALA1`**

:   `Mandant, MerkmalA1`

**`FK_KLASSEN_MERKMALA2`**

:   `Mandant, MerkmalA2`

**`FK_KLASSEN_MERKMALA3`**

:   `Mandant, MerkmalA3`

**`FK_KLASSEN_MERKMALA4`**

:   `Mandant, MerkmalA4`

**`FK_KLASSEN_MERKMALA5`**

:   `Mandant, MerkmalA5`

**`FK_KLASSEN_MERKMALA6`**

:   `Mandant, MerkmalA6`

**`FK_KLASSEN_MERKMALS1`**

:   `Mandant, MerkmalS1`

**`FK_KLASSEN_MERKMALS2`**

:   `Mandant, MerkmalS2`

**`FK_KLASSEN_MERKMALS3`**

:   `Mandant, MerkmalS3`

**`FK_KLASSEN_MERKMALS4`**

:   `Mandant, MerkmalS4`

**`FK_KLASSEN_NAECHSTEKLASSE`**

:   `Mandant, NaechsteKlasse`

**`FK_KLASSEN_NAECHSTEKLASSEZ`**

:   `NaechsteKlasseZeitraum`

**`FK_KLASSEN_ORGANISATION`**

:   `Organisation`

**`FK_KLASSEN_SCHULART`**

:   `Schulart`

**`FK_KLASSEN_SCHULFORM`**

:   `Schulform`

**`FK_KLASSEN_SCHULSTELLE`**

:   `Schulstelle`

**`FK_KLASSE_FOERDERSCHWERP1`**

:   `FoerderSchwerpunkt1`

**`FK_KLASSE_FOERDERSCHWERP2`**

:   `FoerderSchwerpunkt2`

**`PK_KLASSEN`**

:   `Mandant, ID`
