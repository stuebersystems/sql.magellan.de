# Tabelle **SchuelerSorgebe**

## Spalten

Diese Tabelle hat 20 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Sorgeberechtigte](../../tables/sorgeberechtigte)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Sorgebe`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Sorgeberechtigte](../../tables/sorgeberechtigte)

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Person`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Personen](../../tables/personen)

**`Geschwister`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Familiennr`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Verhaeltnis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Mutter
    1 | Vater
    2 | Eltern
    3 | Erziehungsberechtigte\(r\)
    4 | Sorgeberechtigte\(r\)
    5 | Ansprechpartner\(in\)
    6 | Vormund
    7 | Großmutter
    8 | Großvater
    9 | Pflegeeltern
    11 | Verhältnis1
    12 | Verhältnis2
    13 | Verhältnis3
    14 | Verhältnis4
    15 | Verhältnis5
    16 | Verhältnis6
    17 | Verhältnis7
    18 | Verhältnis8
    19 | Verhältnis9
    20 | Verhältnis10
    11\-20 | Werte können in Magellan angepasst werden
    21 | Onkel
    22 | Tante
    23 | Bruder
    24 | Schwester
    25 | Erzieher
    26 | Notfall
    27 | Gasteltern

**`Sorgerecht`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `DEFAULT 'N'`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Hauptversicherter`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Benachrichtigung`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Immer
    1 | Nur im Notfall
    2 | Nie

**`SeriendruckName1`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`SeriendruckName2`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Briefempfaenger`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Briefanrede`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`TelefonPrioritaet`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Telefon privat
    1 | Telefon Beruf
    2 | Mobil

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerSorgebe`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 4 Fremdschlüssel.

**`FK_SCHUELERSB_LEHRER`**

:   `Lehrer, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERSB_PERSON`**

:   `Mandant, Person` » [`Personen (ID, Mandant)`](../../tables/personen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERSB_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERSB_SORGEBE`**

:   `Mandant, Sorgebe` » [`Sorgeberechtigte (ID, Mandant)`](../../tables/sorgeberechtigte) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 6 Indizes.

**`FK_SCHUELERSB_GESCHWISTER`**

:   `Mandant, Geschwister`

**`FK_SCHUELERSB_LEHRER`**

:   `Mandant, Lehrer`

**`FK_SCHUELERSB_PERSON`**

:   `Mandant, Person`

**`FK_SCHUELERSB_SCHUELER`**

:   `Mandant, Schueler`

**`FK_SCHUELERSB_SORGEBE`**

:   `Mandant, Sorgebe`

**`PK_SCHUELERSB`**

:   `Mandant, ID`
