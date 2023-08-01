# Tabelle **Schueler**

## Spalten

Diese Tabelle hat 302 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`GUID`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`IDIntern`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`IDExtern`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`GUIDExtern`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Barcode`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BarcodePrint`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Nachname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`NachnameNative`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Namenszusatz`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`NamenszusatzNative`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Vorname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`VornameNative`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Vorname2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Vorname2Native`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Anrede`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    0 | Frau
    1 | Herr
    2 | Frau Dr\.
    3 | Herr Dr\.
    4 | Frau Prof\.
    5 | Herr Prof\.
    6 | Frau Prof\. Dr\.
    7 | Herr Prof\. Dr\.
    : | Ms\.
    ; | Mrs\.
    < | Mr\.

**`Geschlecht`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    W | Weiblich
    M | Weiblich
    D | Divers

**`Geburtsdatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Geburtsort`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Geburtskreis`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Geburtsland`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Staatsangehoerigkeiten](../../tables/staatsangehoerigkeiten)

**`Geburtsname`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Strasse`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Adresszusatz`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Land`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`PLZ`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Ort`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Ortsteil`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Adressgebiet`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Gemeinde`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Gemeinden](../../tables/gemeinden)

**`Stadtbezirk`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Stadtbezirke](../../tables/stadtbezirke)

**`Telefon`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Telefax`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Mobil`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`EMail`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Wohnform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Wohnformen](../../tables/wohnformen)

**`Staatsangeh1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Staatsangehoerigkeiten](../../tables/staatsangehoerigkeiten)

**`Staatsangeh2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Staatsangehoerigkeiten](../../tables/staatsangehoerigkeiten)

**`Muttersprache`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Muttersprachen](../../tables/muttersprachen)

**`Verkehrssprache`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Muttersprachen](../../tables/muttersprachen)

**`Sprachgruppe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Sprachgruppen](../../tables/sprachgruppen)

**`NichtDeutscheHerkunft`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Aussiedler`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`AussiedlerSeit`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Auslaender`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`AuslaenderSeit`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`InDeutschlandSeit`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`AufenthaltserlaubnisVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`AufenthaltserlaubnisBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Konfession`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Konfessionen](../../tables/konfessionen)

**`RelWunsch`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [RelWuensche](../../tables/relwuensche)

**`RelTeilnahme`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [RelTeilnahmen](../../tables/relteilnahmen)

**`RelGrund`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [RelGruende](../../tables/relgruende)

**`RelAbmeldungVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`RelAbmeldungBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Umschulung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Umschulungsmerkmale](../../tables/umschulungsmerkmale)

**`Funktion1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)

**`Funktion2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)

**`Funktion3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)

**`Funktion4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)

**`Funktion5`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)

**`Funktion6`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)

**`Funktion7`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)

**`Funktion8`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)

**`Personalnr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Krankenkasse`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Krankenkassen](../../tables/krankenkassen)

**`Versicherungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Versicherungsarten](../../tables/versicherungsarten)

**`NotfallPerson`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`NotfallTelefon`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Fahrschueler`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Fahrstrecke`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`FahrstreckeKM`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Einstiegsstelle`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Verkehrsmittel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Verkehrsmittel](../../tables/verkehrsmittel)

**`Fahrgeld`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`FahrgeldbewVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`FahrgeldbewBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Fahrkarte`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fahrkarten](../../tables/fahrkarten)

**`FahrkarteGueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`FahrkarteGueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`KFZ`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Anmeldestatus`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | LABO
    1 | Angemeldet \(und angenommen\)
    2 | AAG \(Antrag, Aufnahme an andere Grundschule\)

**`Profil`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerProfile](../../tables/schuelerprofile)

**`SchulpflichtErfuellt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Bafoeg`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`BafoegBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Foerderzentrum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Integrationsschueler`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Gastschueler`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`GastschulgeldUeberwiesen`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Bildungskarte`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | B1 \(Berlin\)
    1 | B2 \(Berlin\)
    2 | L \(Berlin\)

**`BildungskarteBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Foerderung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Foerderungen](../../tables/foerderungen)

**`Foerdernr`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Foerderbetrag`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`Unterstuetzung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterstuetzungen](../../tables/unterstuetzungen)

**`Betreuung`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Heim
    1 | Hort
    2 | Internat

**`BetreuungAdresse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Adressen](../../tables/adressen)

**`MittagessenTeilnahme`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Ganztagbetrieb`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`GanztagbetriebGebunden`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Früh mit Ferien
    1 | Früh und spät mit Ferien
    2 | Spät und Ferien
    3 | Nur Ferienbetreuung

**`GanztagbetriebOffen`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Früh
    1 | Nachmittags
    2 | Früh und nachmittags
    3 | Nachmittags und spät
    4 | Früh, nachmittags und spät
    5 | Nur Ferienbetreuung

**`BewerbungAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Bewerbungsziel1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bewerbungsziele](../../tables/bewerbungsziele)

**`Bewerbungsziel2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bewerbungsziele](../../tables/bewerbungsziele)

**`Bewerbungsziel3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bewerbungsziele](../../tables/bewerbungsziele)

**`Bewerbungsziel4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bewerbungsziele](../../tables/bewerbungsziele)

**`BewerberStatus`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Auf Warteliste
    1 | Angenommen für Bildungsziel 1
    2 | Angenommen für Bildungsziel 2
    3 | Angenommen für Bildungsziel 3
    4 | Nicht angenommen
    5 | Angenommen für Bildungsziel 4
    6 | Beratungstest
    7 | Beratungsgespräch
    8 | Nicht zum Gespräch\/Testerschienen
    9 | Aufnahmebescheid
    10 | Zusage nicht zurück
    11 | Abgemeldet
    12 | Rückmeldung

**`BewerberHFNote`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfächerdurchschnitt

**`BewerberStatusAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`BewerberNote`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Gesamtdurchschnitt

**`BewerberPunkte`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`BewerberRangzahlZiel1`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`BewerberRangzahlZiel2`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`BewerberRangzahlZiel3`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`BewerberRangzahlZiel4`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`BewerberRangzahl`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Fremdsprache1Von`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache1Bis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache1Note`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Fremdsprache1Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Auf Warteliste
    1 | Angenommen für Bildungsziel 1
    2 | Angenommen für Bildungsziel 2
    3 | Angenommen für Bildungsziel 3
    4 | Nicht angenommen
    5 | Angenommen für Bildungsziel 4
    6 | Beratungstest
    7 | Beratungsgespräch

**`Fremdsprache1Status2`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Pflichtfach\/Wahlpflichtfach
    1 | Wahlfach \(fakultative FS
    2 | Arbeitsgemeinschaft
    3 | Förderunterricht
    4 | Pflichtfach
    5 | Wahlpflichtfach
    6 | Neigungsunterricht
    7 | Muttersprachl\. Unterricht
    8 | Basiskurs
    9 | Erweiterungskurs
    10 | Gymnasialkurs

**`Fremdsprache1Referenz`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Sprachreferenzen](../../tables/sprachreferenzen)

**`Fremdsprache2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Fremdsprache2Von`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache2Bis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache2Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Auf Warteliste
    1 | Angenommen für Bildungsziel 1
    2 | Angenommen für Bildungsziel 2
    3 | Angenommen für Bildungsziel 3
    4 | Nicht angenommen
    5 | Angenommen für Bildungsziel 4
    6 | Beratungstest
    7 | Beratungsgespräch

**`Fremdsprache2Status2`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Pflichtfach\/Wahlpflichtfach
    1 | Wahlfach \(fakultative FS
    2 | Arbeitsgemeinschaft
    3 | Förderunterricht
    4 | Pflichtfach
    5 | Wahlpflichtfach
    6 | Neigungsunterricht
    7 | Muttersprachl\. Unterricht
    8 | Basiskurs
    9 | Erweiterungskurs
    10 | Gymnasialkurs

**`Fremdsprache2Note`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Fremdsprache2Referenz`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Sprachreferenzen](../../tables/sprachreferenzen)

**`Fremdsprache3`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Fremdsprache3Von`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache3Bis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache3Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Auf Warteliste
    1 | Angenommen für Bildungsziel 1
    2 | Angenommen für Bildungsziel 2
    3 | Angenommen für Bildungsziel 3
    4 | Nicht angenommen
    5 | Angenommen für Bildungsziel 4
    6 | Beratungstest
    7 | Beratungsgespräch

**`Fremdsprache3Status2`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Pflichtfach\/Wahlpflichtfach
    1 | Wahlfach \(fakultative FS
    2 | Arbeitsgemeinschaft
    3 | Förderunterricht
    4 | Pflichtfach
    5 | Wahlpflichtfach
    6 | Neigungsunterricht
    7 | Muttersprachl\. Unterricht
    8 | Basiskurs
    9 | Erweiterungskurs
    10 | Gymnasialkurs

**`Fremdsprache3Note`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Fremdsprache3Referenz`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Sprachreferenzen](../../tables/sprachreferenzen)

**`Fremdsprache4`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Fremdsprache4Von`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache4Bis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fremdsprache4Note`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Fremdsprache4Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Auf Warteliste
    1 | Angenommen für Bildungsziel 1
    2 | Angenommen für Bildungsziel 2
    3 | Angenommen für Bildungsziel 3
    4 | Nicht angenommen
    5 | Angenommen für Bildungsziel 4
    6 | Beratungstest
    7 | Beratungsgespräch

**`Fremdsprache4Status2`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Pflichtfach\/Wahlpflichtfach
    1 | Wahlfach \(fakultative FS
    2 | Arbeitsgemeinschaft
    3 | Förderunterricht
    4 | Pflichtfach
    5 | Wahlpflichtfach
    6 | Neigungsunterricht
    7 | Muttersprachl\. Unterricht
    8 | Basiskurs
    9 | Erweiterungskurs
    10 | Gymnasialkurs

**`Fremdsprache4Referenz`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Sprachreferenzen](../../tables/sprachreferenzen)

**`Ausbildung`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [SchuelerAusbildung](../../tables/schuelerausbildung)

**`G8G9`**

:   [`VARCHAR(2)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Latinum`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Graecum`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HoechsterBildungsgangABS`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bildungsgaenge](../../tables/bildungsgaenge)

**`HoechsterAbschlussABSSchulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchulformenHerkunft](../../tables/schulformenherkunft)

**`HoechsterAbschlussABS`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [AbschluesseExtern](../../tables/abschluesseextern)

**`HoechsterAbschlussABSAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`HoechsterAbschlussABSSchule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`HoechsterAbschlussABSNote`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`HoechsterBildungsgangBBS`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bildungsgaenge](../../tables/bildungsgaenge)

**`HoechsterAbschlussBBSSchulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchulformenHerkunft](../../tables/schulformenherkunft)

**`HoechsterAbschlussBBS`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [AbschluesseExtern](../../tables/abschluesseextern)

**`HoechsterAbschlussBBSBeruf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Berufe](../../tables/berufe)

**`HoechsterAbschlussBBSBerufAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`HoechsterAbschlussBBSSchule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`HoechsterAbschlussBBSAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`HoechsterAbschlussBBSAustritt`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Abschluss
    1 | Abgang
    2 | Abbruch

**`HoechsterAbschlussBBSNote`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Berufsjahre`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`HerkunftSchule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [SchuelerSchulen](../../tables/schuelerschulen)

**`ZugangAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Zugang2Am`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Grundschuleintritt`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Einschulung`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    1 | Vorzeitige Einschulung
    2 | Fristgerechte Einschulung
    3 | Verspätete Einschulung

**`EinschulungAntrag`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`EinschulungAbgebendeSchule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Einschulmerkmal`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Einschulmerkmale](../../tables/einschulmerkmale)

**`Einschulmerkmal2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Einschulmerkmale](../../tables/einschulmerkmale)

**`Einschulmerkmal3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Einschulmerkmale](../../tables/einschulmerkmale)

**`EinschulungBemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`VoraussichtlichesEnde`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Ueberweisung`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`UeberweisungAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Abgang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abgangsarten](../../tables/abgangsarten)

**`AbgangAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Abgang2Am`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Uebergang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Uebergangsarten](../../tables/uebergangsarten)

**`UebergangAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`UebergangAnSchule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`UebergangAnSchulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchulformenUebergang](../../tables/schulformenuebergang)

**`UebergangKlassenstufe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Klassenstufen](../../tables/klassenstufen)

**`UebergangUnterlagen`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`UebergangFoerderUnterlagen`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`UebergangZeugnis`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`UebergangGeaendertAm`**

:   [`TIMESTAMP`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`UebergangGeaendertVon`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Passfoto`**

:   [`BLOB subtype binary`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`MerkmalA1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalA2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalA3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalA4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalA5`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalA6`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS5`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS6`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS7`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS8`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS10`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalS9`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerMerkmale](../../tables/schuelermerkmale)

**`MerkmalB1`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB3`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB4`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalT1`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalT2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalT3`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalT4`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalD1`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`MerkmalD2`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`MerkmalD3`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`MerkmalD4`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`MerkmalU1`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`MerkmalU2`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Auskunft`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Keine Angabe
    1 | Geheim

**`AuswaertigerSchueler`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerArten](../../tables/schuelerarten)

**`AusstellungBehoerde`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`AusstellungBehoerdeDatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`BetreuungInnerschulisch1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [BetreuungenInnerschulisch](../../tables/betreuungeninnerschulisch)

**`BetreuungInnerschulisch2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [BetreuungenInnerschulisch](../../tables/betreuungeninnerschulisch)

**`BetreuungInnerschulisch3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [BetreuungenInnerschulisch](../../tables/betreuungeninnerschulisch)

**`BetreuungAusserschulisch1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [BetreuungenAusserschulisch](../../tables/betreuungenausserschulisch)

**`BetreuungAusserschulisch2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [BetreuungenAusserschulisch](../../tables/betreuungenausserschulisch)

**`BetreuungAusserschulisch3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [BetreuungenAusserschulisch](../../tables/betreuungenausserschulisch)

**`AkteAngefordert`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`LMAnteil`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Lernmittelanteil in Prozent vom Regelbeitrag

**`LMZahlungsstand`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Unbezahlt
    1 | Mahnung 1
    2 | Mahnung 2
    3 | Mahnung 3
    4 | Bezahlt
    5 | Teilbezahlt

**`LMZahlungsstandDatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`LMBefreit`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`LMBefreitBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`LMZusatzbeitrag`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`AusweisAusgestelltAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`AusweisBemerkung`**

:   [`VARCHAR(150)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Wahlfach1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Wahlfach2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Wahlfach3`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Wahlfach4`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Wahlfach5`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Wahlfach6`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`SchuelerausweisBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`BLZ`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Bank`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Banken](../../tables/banken)

**`Bankkonto`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BankIBAN`**

:   [`VARCHAR(28)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BankInhaber`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BankInfo`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BankBemerkung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Banken](../../tables/banken)

**`Bank2konto`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank2IBAN`**

:   [`VARCHAR(28)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank2Inhaber`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank2Info`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank2Bemerkung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1Name1`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1Name2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1Strasse`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1Adressgebiet`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1Land`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1PLZ`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1Ort`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1Ortsteil`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung1Adresszusatz`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2Name1`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2Name2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2Strasse`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2Adressgebiet`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2Land`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2PLZ`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2Ort`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2Ortsteil`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Rechnung2Adresszusatz`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatName1`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatName2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatStrasse`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatAdressgebiet`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatLand`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatPLZ`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatOrt`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatOrtsteil`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatAdresszusatz`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatGemeinde`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Gemeinden](../../tables/gemeinden)

**`PassNr`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`PassGueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`VisumNr`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`VisumAblaufAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`VisumAusstellungsort`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Sozialversicherungsnummer`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Aufenthaltsbemerkung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`SYNC`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Schueler`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 49 Fremdschlüssel.

**`FK_SCHUELER_ABSCHLUSSABS`**

:   `HoechsterAbschlussABS` » [`AbschluesseExtern (Kuerzel)`](../../tables/abschluesseextern) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_ABSCHLUSSABSSCHULE`**

:   `HoechsterAbschlussABSSchule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_ABSCHLUSSABSSCHULF`**

:   `HoechsterAbschlussABSSchulform` » [`SchulformenHerkunft (Kuerzel)`](../../tables/schulformenherkunft) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_ABSCHLUSSBBS`**

:   `HoechsterAbschlussBBS` » [`AbschluesseExtern (Kuerzel)`](../../tables/abschluesseextern) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_ABSCHLUSSBBSBERUF`**

:   `HoechsterAbschlussBBSBeruf` » [`Berufe (Kuerzel)`](../../tables/berufe) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_ABSCHLUSSBBSSCHULE`**

:   `HoechsterAbschlussBBSSchule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_ABSCHLUSSBBSSCHULF`**

:   `HoechsterAbschlussBBSSchulform` » [`SchulformenHerkunft (Kuerzel)`](../../tables/schulformenherkunft) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_AUSBILDUNG`**

:   `Ausbildung, Mandant` » [`SchuelerAusbildung (ID, Mandant)`](../../tables/schuelerausbildung) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

**`FK_SCHUELER_AUSWAERTIG`**

:   `AuswaertigerSchueler` » [`SchuelerArten (Kuerzel)`](../../tables/schuelerarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_BANK`**

:   `Bank` » [`Banken (ID)`](../../tables/banken) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_BANK2`**

:   `Bank2` » [`Banken (ID)`](../../tables/banken) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_BETREUUNGADRESSE`**

:   `BetreuungAdresse, Mandant` » [`Adressen (ID, Mandant)`](../../tables/adressen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_BETREUUNGAUSSER1`**

:   `BetreuungAusserschulisch1` » [`BetreuungenAusserschulisch (Kuerzel)`](../../tables/betreuungenausserschulisch) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_BETREUUNGAUSSER2`**

:   `BetreuungAusserschulisch2` » [`BetreuungenAusserschulisch (Kuerzel)`](../../tables/betreuungenausserschulisch) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_BETREUUNGAUSSER3`**

:   `BetreuungAusserschulisch3` » [`BetreuungenAusserschulisch (Kuerzel)`](../../tables/betreuungenausserschulisch) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_BETREUUNGINNER1`**

:   `BetreuungInnerschulisch1` » [`BetreuungenInnerschulisch (Kuerzel)`](../../tables/betreuungeninnerschulisch) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_BETREUUNGINNER2`**

:   `BetreuungInnerschulisch2` » [`BetreuungenInnerschulisch (Kuerzel)`](../../tables/betreuungeninnerschulisch) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_BETREUUNGINNER3`**

:   `BetreuungInnerschulisch3` » [`BetreuungenInnerschulisch (Kuerzel)`](../../tables/betreuungeninnerschulisch) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_BLDGABS`**

:   `HoechsterBildungsgangABS` » [`Bildungsgaenge (Kuerzel)`](../../tables/bildungsgaenge) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_BLDGBBS`**

:   `HoechsterBildungsgangBBS` » [`Bildungsgaenge (Kuerzel)`](../../tables/bildungsgaenge) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_EINSCHABGSCHULE`**

:   `EinschulungAbgebendeSchule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_EINSCHULMERKMAL`**

:   `Einschulmerkmal` » [`Einschulmerkmale (Kuerzel)`](../../tables/einschulmerkmale) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_EINSCHULMERKMAL2`**

:   `Einschulmerkmal2` » [`Einschulmerkmale (Kuerzel)`](../../tables/einschulmerkmale) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_EINSCHULMERKMAL3`**

:   `Einschulmerkmal3` » [`Einschulmerkmale (Kuerzel)`](../../tables/einschulmerkmale) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_FAHRKARTE`**

:   `Fahrkarte` » [`Fahrkarten (Kuerzel)`](../../tables/fahrkarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_FOERDERUNG`**

:   `Foerderung` » [`Foerderungen (Kuerzel)`](../../tables/foerderungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_FOERDERZENTRUM`**

:   `Foerderzentrum` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_FSP1REF`**

:   `Fremdsprache1Referenz` » [`Sprachreferenzen (Kuerzel)`](../../tables/sprachreferenzen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_FSP2REF`**

:   `Fremdsprache2Referenz` » [`Sprachreferenzen (Kuerzel)`](../../tables/sprachreferenzen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_FSP3REF`**

:   `Fremdsprache3Referenz` » [`Sprachreferenzen (Kuerzel)`](../../tables/sprachreferenzen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_FSP4REF`**

:   `Fremdsprache4Referenz` » [`Sprachreferenzen (Kuerzel)`](../../tables/sprachreferenzen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_GEBURTSLAND`**

:   `Geburtsland` » [`Staatsangehoerigkeiten (Kuerzel)`](../../tables/staatsangehoerigkeiten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_GEMEINDE`**

:   `Gemeinde` » [`Gemeinden (Schluessel)`](../../tables/gemeinden) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_HEIMATGEMEINDE`**

:   `HeimatGemeinde` » [`Gemeinden (Schluessel)`](../../tables/gemeinden) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_KRANKENKASSE`**

:   `Krankenkasse` » [`Krankenkassen (Kuerzel)`](../../tables/krankenkassen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELER_MUTTERSPRACHE`**

:   `Muttersprache` » [`Muttersprachen (Kuerzel)`](../../tables/muttersprachen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_PROFIL`**

:   `Profil` » [`SchuelerProfile (Kuerzel)`](../../tables/schuelerprofile) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_SPRACHGRUPPE`**

:   `Sprachgruppe` » [`Sprachgruppen (Kuerzel)`](../../tables/sprachgruppen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_UEBERGANG`**

:   `Uebergang` » [`Uebergangsarten (Kuerzel)`](../../tables/uebergangsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_UEBERGANGSCHULE`**

:   `UebergangAnSchule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_UEBERGANGSCHULFORM`**

:   `UebergangAnSchulform` » [`SchulformenUebergang (Kuerzel)`](../../tables/schulformenuebergang) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_UEBKLASSENSTUFE`**

:   `UebergangKlassenstufe` » [`Klassenstufen (Kuerzel)`](../../tables/klassenstufen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHUELER_UMSCHULUNG`**

:   `Umschulung` » [`Umschulungsmerkmale (Kuerzel)`](../../tables/umschulungsmerkmale) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_UNTERSTUETZUNG`**

:   `Unterstuetzung` » [`Unterstuetzungen (Kuerzel)`](../../tables/unterstuetzungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_VERKEHRSMITTEL`**

:   `Verkehrsmittel` » [`Verkehrsmittel (Kuerzel)`](../../tables/verkehrsmittel) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_VERKEHRSSPRACHE`**

:   `Verkehrssprache` » [`Muttersprachen (Kuerzel)`](../../tables/muttersprachen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_VERSICHERUNGSART`**

:   `Versicherungsart` » [`Versicherungsarten (Kuerzel)`](../../tables/versicherungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELER_WOHNFORM`**

:   `Wohnform` » [`Wohnformen (Kuerzel)`](../../tables/wohnformen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 76 Indizes.

**`FK_SCHUELER_ABGANG`**

:   `Abgang`

**`FK_SCHUELER_ABSCHLUSSABS`**

:   `HoechsterAbschlussABS`

**`FK_SCHUELER_ABSCHLUSSABSSCHULE`**

:   `HoechsterAbschlussABSSchule`

**`FK_SCHUELER_ABSCHLUSSABSSCHULF`**

:   `HoechsterAbschlussABSSchulform`

**`FK_SCHUELER_ABSCHLUSSBBS`**

:   `HoechsterAbschlussBBS`

**`FK_SCHUELER_ABSCHLUSSBBSBERUF`**

:   `HoechsterAbschlussBBSBeruf`

**`FK_SCHUELER_ABSCHLUSSBBSSCHULE`**

:   `HoechsterAbschlussBBSSchule`

**`FK_SCHUELER_ABSCHLUSSBBSSCHULF`**

:   `HoechsterAbschlussBBSSchulform`

**`FK_SCHUELER_AUSBILDUNG`**

:   `Mandant, Ausbildung`

**`FK_SCHUELER_AUSWAERTIG`**

:   `AuswaertigerSchueler`

**`FK_SCHUELER_BANK`**

:   `Bank`

**`FK_SCHUELER_BANK2`**

:   `Bank2`

**`FK_SCHUELER_BETREUUNGADRESSE`**

:   `Mandant, BetreuungAdresse`

**`FK_SCHUELER_BETREUUNGAUSSER1`**

:   `BetreuungAusserschulisch1`

**`FK_SCHUELER_BETREUUNGAUSSER2`**

:   `BetreuungAusserschulisch2`

**`FK_SCHUELER_BETREUUNGAUSSER3`**

:   `BetreuungAusserschulisch3`

**`FK_SCHUELER_BETREUUNGINNER1`**

:   `BetreuungInnerschulisch1`

**`FK_SCHUELER_BETREUUNGINNER2`**

:   `BetreuungInnerschulisch2`

**`FK_SCHUELER_BETREUUNGINNER3`**

:   `BetreuungInnerschulisch3`

**`FK_SCHUELER_BLDGABS`**

:   `HoechsterBildungsgangABS`

**`FK_SCHUELER_BLDGBBS`**

:   `HoechsterBildungsgangBBS`

**`FK_SCHUELER_EINSCHABGSCHULE`**

:   `EinschulungAbgebendeSchule`

**`FK_SCHUELER_EINSCHULMERKMAL`**

:   `Einschulmerkmal`

**`FK_SCHUELER_EINSCHULMERKMAL2`**

:   `Einschulmerkmal2`

**`FK_SCHUELER_EINSCHULMERKMAL3`**

:   `Einschulmerkmal3`

**`FK_SCHUELER_FAHRKARTE`**

:   `Fahrkarte`

**`FK_SCHUELER_FOERDERUNG`**

:   `Foerderung`

**`FK_SCHUELER_FOERDERZENTRUM`**

:   `Foerderzentrum`

**`FK_SCHUELER_FSP1REF`**

:   `Fremdsprache1Referenz`

**`FK_SCHUELER_FSP2REF`**

:   `Fremdsprache2Referenz`

**`FK_SCHUELER_FSP3REF`**

:   `Fremdsprache3Referenz`

**`FK_SCHUELER_FSP4REF`**

:   `Fremdsprache4Referenz`

**`FK_SCHUELER_GEBURTSLAND`**

:   `Geburtsland`

**`FK_SCHUELER_GEMEINDE`**

:   `Gemeinde`

**`FK_SCHUELER_HEIMATGEMEINDE`**

:   `HeimatGemeinde`

**`FK_SCHUELER_KRANKENKASSE`**

:   `Krankenkasse`

**`FK_SCHUELER_MANDANT`**

:   `Mandant`

**`FK_SCHUELER_MUTTERSPRACHE`**

:   `Muttersprache`

**`FK_SCHUELER_PROFIL`**

:   `Profil`

**`FK_SCHUELER_SPRACHGRUPPE`**

:   `Sprachgruppe`

**`FK_SCHUELER_UEBERGANG`**

:   `Uebergang`

**`FK_SCHUELER_UEBERGANGSCHULE`**

:   `UebergangAnSchule`

**`FK_SCHUELER_UEBERGANGSCHULFORM`**

:   `UebergangAnSchulform`

**`FK_SCHUELER_UEBKLASSENSTUFE`**

:   `UebergangKlassenstufe`

**`FK_SCHUELER_UMSCHULUNG`**

:   `Umschulung`

**`FK_SCHUELER_UNTERSTUETZUNG`**

:   `Unterstuetzung`

**`FK_SCHUELER_VERKEHRSMITTEL`**

:   `Verkehrsmittel`

**`FK_SCHUELER_VERKEHRSSPRACHE`**

:   `Verkehrssprache`

**`FK_SCHUELER_VERSICHERUNGSART`**

:   `Versicherungsart`

**`FK_SCHUELER_WOHNFORM`**

:   `Wohnform`

**`IDX_Schueler_Betreuung`**

:   `BetreuungAdresse`

**`IDX_Schueler_Bewerbungsziel1`**

:   `Bewerbungsziel1`

**`IDX_Schueler_Bewerbungsziel2`**

:   `Bewerbungsziel2`

**`IDX_Schueler_Bewerbungsziel3`**

:   `Bewerbungsziel3`

**`IDX_Schueler_Bewerbungsziel4`**

:   `Bewerbungsziel4`

**`IDX_Schueler_FS1`**

:   `Fremdsprache1`

**`IDX_Schueler_FS2`**

:   `Fremdsprache2`

**`IDX_Schueler_FS3`**

:   `Fremdsprache3`

**`IDX_Schueler_FS4`**

:   `Fremdsprache4`

**`IDX_Schueler_Funktion1`**

:   `Funktion1`

**`IDX_Schueler_Funktion2`**

:   `Funktion2`

**`IDX_Schueler_Funktion3`**

:   `Funktion3`

**`IDX_Schueler_Funktion4`**

:   `Funktion4`

**`IDX_Schueler_Funktion5`**

:   `Funktion5`

**`IDX_Schueler_Funktion6`**

:   `Funktion6`

**`IDX_Schueler_Funktion7`**

:   `Funktion7`

**`IDX_Schueler_Funktion8`**

:   `Funktion8`

**`IDX_Schueler_HerkunftSchule`**

:   `HerkunftSchule`

**`IDX_Schueler_Konfession`**

:   `Konfession`

**`IDX_Schueler_RelGrund`**

:   `RelGrund`

**`IDX_Schueler_RelTeilnahme`**

:   `RelTeilnahme`

**`IDX_Schueler_RelWunsch`**

:   `RelWunsch`

**`IDX_Schueler_Staatsangeh1`**

:   `Staatsangeh1`

**`IDX_Schueler_Staatsangeh2`**

:   `Staatsangeh2`

**`IDX_Schueler_Status`**

:   `Status`

**`PK_SCHUELER`**

:   `Mandant, ID`
