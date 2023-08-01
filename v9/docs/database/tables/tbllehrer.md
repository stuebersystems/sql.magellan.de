# Table **tblLehrer**

## Columns

This table contains 171 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

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

**`Kuerzel`**

:   [`VARCHAR(6)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

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

    Value | Description
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

    Value | Description
    - | -
    W | Weiblich
    M | Weiblich
    D | Divers

**`Geburtsdatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Geburtsort`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Geburtsname`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Ehestand`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Value | Description
    - | -
    0 | Verheiratet
    1 | Nicht Verheiratet
    2 | Ledig
    3 | Geschieden
    4 | Verwitwet

**`Kinderzahl`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

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

**`Gemeinde`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Gemeinden](../../tables/gemeinden)

**`Adressgebiet`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Telefon`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Telefax`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Mobil`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Email`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`TelefonDienst`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`TelefaxDienst`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`KFZ1`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`KFZ2`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Kategorie`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Lehrerkategorien](../../tables/lehrerkategorien)

**`Staatsangeh`**

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

**`Konfession`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Konfessionen](../../tables/konfessionen)

**`Bevollmaechtigung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bevollmaechtigungen](../../tables/bevollmaechtigungen)

**`Abteilung1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abteilungen](../../tables/abteilungen)

**`Abteilung2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abteilungen](../../tables/abteilungen)

**`Abteilung3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abteilungen](../../tables/abteilungen)

**`Funktion1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)

**`Funktion1Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion1Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)

**`Funktion2Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion2Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)

**`Funktion3Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion3Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)

**`Funktion4Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion4Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion5`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)

**`Funktion5Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion5Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion6`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)

**`Funktion6Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion6Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion7`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)

**`Funktion7Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion7Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion8`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)

**`Funktion8Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Funktion8Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

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

**`Personalnr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Statistiknr`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`ZugangDatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`ZugangGrund`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerZugaenge](../../tables/lehrerzugaenge)

**`AbgangDatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`AbgangGrund`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Amtsbez`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Amtsbez](../../tables/amtsbez)

**`AmtsbezSeit`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Dienstverh`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Dienstverh](../../tables/dienstverh)

**`Dienstbez`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Dienstbez](../../tables/dienstbez)

**`Dienstherr`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Dienstherren](../../tables/dienstherren)

**`Dienstalter`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`LetzteUeberpruefung`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`VertragVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`VertragBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Beschaeftigungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Beschaeftigungsarten](../../tables/beschaeftigungsarten)

**`Beschaeftigungsverh`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Beschaeftigungsverh](../../tables/beschaeftigungsverh)

**`BeschaeftigungSchulart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schularten](../../tables/schularten)

**`BeschaeftigungSchulzweig`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Schulzweige](../../tables/schulzweige)

**`Besoldung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Besoldungen](../../tables/besoldungen)

**`Ausbildung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerAusbildung](../../tables/lehrerausbildung)

**`Beruf`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Berufe](../../tables/berufe)

**`BerichtendeSchule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Abordnung1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Abordnung1Art`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abordnungsarten](../../tables/abordnungsarten)

**`Abordnung2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Abordnung2Art`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abordnungsarten](../../tables/abordnungsarten)

**`Status`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Inaktiv
    1 | Aktiv

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Passfoto`**

:   [`BLOB subtype binary`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`MerkmalA1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalA2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalA3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalA4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalA5`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalA6`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalS1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalS2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalS3`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalS4`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerMerkmale](../../tables/lehrermerkmale)

**`MerkmalB1`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB2`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB3`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MerkmalB4`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Banken](../../tables/banken)

**`Bank1Konto`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank1IBAN`**

:   [`VARCHAR(28)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank1Inhaber`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank1Info`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank1Bemerkung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Bank2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Banken](../../tables/banken)

**`Bank2Konto`**

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

**`SYNC`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

## Primary key

This table has a primary key.

**`tblLehrer`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_LEHRER_ABORDNUNG1`**

:   `Abordnung1` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_LEHRER_ABORDNUNG1ART`**

:   `Abordnung1Art` » [`Abordnungsarten (Kuerzel)`](../../tables/abordnungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_ABORDNUNG2`**

:   `Abordnung2` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_LEHRER_ABORDNUNG2ART`**

:   `Abordnung2Art` » [`Abordnungsarten (Kuerzel)`](../../tables/abordnungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_ABTEILUNG1`**

:   `Abteilung1, Mandant` » [`Abteilungen (Kuerzel, Mandant)`](../../tables/abteilungen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_ABTEILUNG2`**

:   `Abteilung2, Mandant` » [`Abteilungen (Kuerzel, Mandant)`](../../tables/abteilungen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_ABTEILUNG3`**

:   `Abteilung3, Mandant` » [`Abteilungen (Kuerzel, Mandant)`](../../tables/abteilungen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_AMTSBEZ`**

:   `Amtsbez` » [`Amtsbez (Kuerzel)`](../../tables/amtsbez) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_AUSBILDUNG`**

:   `Ausbildung` » [`LehrerAusbildung (Kuerzel)`](../../tables/lehrerausbildung) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_BANK1`**

:   `Bank1` » [`Banken (ID)`](../../tables/banken) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_LEHRER_BANK2`**

:   `Bank2` » [`Banken (ID)`](../../tables/banken) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_LEHRER_BERICHTENDESCHULE`**

:   `BerichtendeSchule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_LEHRER_BERUF`**

:   `Beruf` » [`Berufe (Kuerzel)`](../../tables/berufe) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_BESCHAEFT_SCHULART`**

:   `BeschaeftigungSchulart` » [`Schularten (Kuerzel)`](../../tables/schularten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_BESCHAEFT_SCHULZWEIG`**

:   `BeschaeftigungSchulzweig` » [`Schulzweige (Kuerzel)`](../../tables/schulzweige) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_BESCHART`**

:   `Beschaeftigungsart` » [`Beschaeftigungsarten (Kuerzel)`](../../tables/beschaeftigungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_BESCHVERH`**

:   `Beschaeftigungsverh` » [`Beschaeftigungsverh (Kuerzel)`](../../tables/beschaeftigungsverh) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_BESOLDUNG`**

:   `Besoldung` » [`Besoldungen (Kuerzel)`](../../tables/besoldungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_BEVOLLMAECHTIGUNG`**

:   `Bevollmaechtigung` » [`Bevollmaechtigungen (Kuerzel)`](../../tables/bevollmaechtigungen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_DIENSTBEZ`**

:   `Dienstbez` » [`Dienstbez (Kuerzel)`](../../tables/dienstbez) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_DIENSTHERR`**

:   `Dienstherr` » [`Dienstherren (Kuerzel)`](../../tables/dienstherren) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_DIENSTVERH`**

:   `Dienstverh` » [`Dienstverh (Kuerzel)`](../../tables/dienstverh) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_FUNKTION1`**

:   `Funktion1` » [`LehrerFunktionen (Kuerzel)`](../../tables/lehrerfunktionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_FUNKTION2`**

:   `Funktion2` » [`LehrerFunktionen (Kuerzel)`](../../tables/lehrerfunktionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_FUNKTION3`**

:   `Funktion3` » [`LehrerFunktionen (Kuerzel)`](../../tables/lehrerfunktionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_FUNKTION4`**

:   `Funktion4` » [`LehrerFunktionen (Kuerzel)`](../../tables/lehrerfunktionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_FUNKTION5`**

:   `Funktion5` » [`LehrerFunktionen (Kuerzel)`](../../tables/lehrerfunktionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_FUNKTION6`**

:   `Funktion6` » [`LehrerFunktionen (Kuerzel)`](../../tables/lehrerfunktionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_FUNKTION7`**

:   `Funktion7` » [`LehrerFunktionen (Kuerzel)`](../../tables/lehrerfunktionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_FUNKTION8`**

:   `Funktion8` » [`LehrerFunktionen (Kuerzel)`](../../tables/lehrerfunktionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_GEMEINDE`**

:   `Gemeinde` » [`Gemeinden (Schluessel)`](../../tables/gemeinden) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_HEIMATGEMEINDE`**

:   `HeimatGemeinde` » [`Gemeinden (Schluessel)`](../../tables/gemeinden) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_KATEGORIE`**

:   `Kategorie` » [`Lehrerkategorien (Kuerzel)`](../../tables/lehrerkategorien) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_KONFESSION`**

:   `Konfession` » [`Konfessionen (Kuerzel)`](../../tables/konfessionen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_KRANKENKASSE`**

:   `Krankenkasse` » [`Krankenkassen (Kuerzel)`](../../tables/krankenkassen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MANDANT`**

:   `Mandant` » [`Mandanten (ID)`](../../tables/mandanten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALA1`**

:   `Mandant, MerkmalA1` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALA2`**

:   `Mandant, MerkmalA2` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALA3`**

:   `Mandant, MerkmalA3` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALA4`**

:   `Mandant, MerkmalA4` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALA5`**

:   `Mandant, MerkmalA5` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALA6`**

:   `Mandant, MerkmalA6` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALS1`**

:   `Mandant, MerkmalS1` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALS2`**

:   `Mandant, MerkmalS2` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALS3`**

:   `Mandant, MerkmalS3` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MERKMALS4`**

:   `Mandant, MerkmalS4` » [`LehrerMerkmale (Kuerzel, Mandant)`](../../tables/lehrermerkmale) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_MUTTERSPRACHE`**

:   `Muttersprache` » [`Muttersprachen (Kuerzel)`](../../tables/muttersprachen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_STAATSANGEH1`**

:   `Staatsangeh` » [`Staatsangehoerigkeiten (Kuerzel)`](../../tables/staatsangehoerigkeiten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_STAATSANGEH2`**

:   `Staatsangeh2` » [`Staatsangehoerigkeiten (Kuerzel)`](../../tables/staatsangehoerigkeiten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_VERKEHRSSPRACHE`**

:   `Verkehrssprache` » [`Muttersprachen (Kuerzel)`](../../tables/muttersprachen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_LEHRER_VERSART`**

:   `Versicherungsart` » [`Versicherungsarten (Kuerzel)`](../../tables/versicherungsarten) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_LEHRER_ZUGANG`**

:   `ZugangGrund` » [`LehrerZugaenge (Kuerzel)`](../../tables/lehrerzugaenge) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

## Indices

This table has 62 indices.

**`FK_LEHRER_ABGANG`**

:   `AbgangGrund`

**`FK_LEHRER_ABORDNUNG1`**

:   `Abordnung1`

**`FK_LEHRER_ABORDNUNG1ART`**

:   `Abordnung1Art`

**`FK_LEHRER_ABORDNUNG2`**

:   `Abordnung2`

**`FK_LEHRER_ABORDNUNG2ART`**

:   `Abordnung2Art`

**`FK_LEHRER_ABTEILUNG1`**

:   `Mandant, Abteilung1`

**`FK_LEHRER_ABTEILUNG2`**

:   `Mandant, Abteilung2`

**`FK_LEHRER_ABTEILUNG3`**

:   `Mandant, Abteilung3`

**`FK_LEHRER_AMTSBEZ`**

:   `Amtsbez`

**`FK_LEHRER_AUSBILDUNG`**

:   `Ausbildung`

**`FK_LEHRER_BANK1`**

:   `Bank1`

**`FK_LEHRER_BANK2`**

:   `Bank2`

**`FK_LEHRER_BERICHTENDESCHULE`**

:   `BerichtendeSchule`

**`FK_LEHRER_BERUF`**

:   `Beruf`

**`FK_LEHRER_BESCHAEFT_SCHULART`**

:   `BeschaeftigungSchulart`

**`FK_LEHRER_BESCHAEFT_SCHULZWEIG`**

:   `BeschaeftigungSchulzweig`

**`FK_LEHRER_BESCHART`**

:   `Beschaeftigungsart`

**`FK_LEHRER_BESCHVERH`**

:   `Beschaeftigungsverh`

**`FK_LEHRER_BESOLDUNG`**

:   `Besoldung`

**`FK_LEHRER_BEVOLLMAECHTIGUNG`**

:   `Bevollmaechtigung`

**`FK_LEHRER_DIENSTBEZ`**

:   `Dienstbez`

**`FK_LEHRER_DIENSTHERR`**

:   `Dienstherr`

**`FK_LEHRER_DIENSTVERH`**

:   `Dienstverh`

**`FK_LEHRER_FUNKTION1`**

:   `Funktion1`

**`FK_LEHRER_FUNKTION2`**

:   `Funktion2`

**`FK_LEHRER_FUNKTION3`**

:   `Funktion3`

**`FK_LEHRER_FUNKTION4`**

:   `Funktion4`

**`FK_LEHRER_FUNKTION5`**

:   `Funktion5`

**`FK_LEHRER_FUNKTION6`**

:   `Funktion6`

**`FK_LEHRER_FUNKTION7`**

:   `Funktion7`

**`FK_LEHRER_FUNKTION8`**

:   `Funktion8`

**`FK_LEHRER_GEMEINDE`**

:   `Gemeinde`

**`FK_LEHRER_HEIMATGEMEINDE`**

:   `HeimatGemeinde`

**`FK_LEHRER_KATEGORIE`**

:   `Kategorie`

**`FK_LEHRER_KONFESSION`**

:   `Konfession`

**`FK_LEHRER_KRANKENKASSE`**

:   `Krankenkasse`

**`FK_LEHRER_MANDANT`**

:   `Mandant`

**`FK_LEHRER_MERKMALA1`**

:   `Mandant, MerkmalA1`

**`FK_LEHRER_MERKMALA2`**

:   `Mandant, MerkmalA2`

**`FK_LEHRER_MERKMALA3`**

:   `Mandant, MerkmalA3`

**`FK_LEHRER_MERKMALA4`**

:   `Mandant, MerkmalA4`

**`FK_LEHRER_MERKMALA5`**

:   `Mandant, MerkmalA5`

**`FK_LEHRER_MERKMALA6`**

:   `Mandant, MerkmalA6`

**`FK_LEHRER_MERKMALS1`**

:   `Mandant, MerkmalS1`

**`FK_LEHRER_MERKMALS2`**

:   `Mandant, MerkmalS2`

**`FK_LEHRER_MERKMALS3`**

:   `Mandant, MerkmalS3`

**`FK_LEHRER_MERKMALS4`**

:   `Mandant, MerkmalS4`

**`FK_LEHRER_MUTTERSPRACHE`**

:   `Muttersprache`

**`FK_LEHRER_STAATSANGEH1`**

:   `Staatsangeh`

**`FK_LEHRER_STAATSANGEH2`**

:   `Staatsangeh2`

**`FK_LEHRER_VERKEHRSSPRACHE`**

:   `Verkehrssprache`

**`FK_LEHRER_VERSART`**

:   `Versicherungsart`

**`FK_LEHRER_ZUGANG`**

:   `ZugangGrund`

**`IDX_Lehrer_Funktion4`**

:   `Funktion4`

**`IDX_Lehrer_Funktion5`**

:   `Funktion5`

**`IDX_Lehrer_Funktion6`**

:   `Funktion6`

**`IDX_Lehrer_Funktion7`**

:   `Funktion7`

**`IDX_Lehrer_Funktion8`**

:   `Funktion8`

**`IDX_Lehrer_Konfession`**

:   `Konfession`

**`IDX_Lehrer_Kuerzel`**

:   `Kuerzel`

**`IDX_Lehrer_Staatsangeh`**

:   `Staatsangeh`

**`PK_LEHRER`**

:   `Mandant, ID`
