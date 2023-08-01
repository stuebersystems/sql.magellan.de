# Tabelle **FachtafelFaecher**

## Spalten

Diese Tabelle hat 40 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Fachtafel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Fachtafeln](../../tables/fachtafeln)

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Fachstatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachstati](../../tables/fachstati)

**`Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`Schwerpunkt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachschwerpunkte](../../tables/fachschwerpunkte)

**`KursNr`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Kursnummer

**`Faktor`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Faktor

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Freies Merkmal

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Zusatzklasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`IstStammkurs`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Ist dies ein Stammkurs?

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Endnote1Fortschreiben`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Soll die Endnote fortgeschrieben werden?

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Soll`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Sollwert \(= Soll aus DAVINCI\)

**`Angleichung`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Angleichungswert \(= Angleichung aus DAVINCI\)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

    Bemerkung

**`Niveau`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [FachNiveaus](../../tables/fachniveaus)

**`Hauptfach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Pflichtkurse`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Anzahl der Pflichtkurse bei Fachwahl

**`HJ1_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    E1 gewählt bei Fachwahl

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ2_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    E2 gewählt bei Fachwahl

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ3_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Q1 gewählt bei Fachwahl

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ4_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Q2 gewählt bei Fachwahl

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ5_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Q3 gewählt bei Fachwahl

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ6_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Q3 gewählt bei Fachwahl

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Q1Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Q2Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Q3Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Q4Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ1_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ2_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ3_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ4_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ5_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ6_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Leistungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Leistungsarten](../../tables/leistungsarten)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`FachtafelFaecher`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 12 Fremdschlüssel.

**`FK_FACHTAFELFAECHER_FACHSTATUS`**

:   `Fachstatus` » [`Fachstati (Kuerzel)`](../../tables/fachstati) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_FACHTAFELFAECHER_FACHTAFEL`**

:   `Fachtafel, Mandant` » [`Fachtafeln (Kuerzel, Mandant)`](../../tables/fachtafeln) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_FACHTAFELFAECHER_HAUPTFACH`**

:   `Hauptfach, Mandant` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_FACHTAFELFAECHER_LART`**

:   `Leistungsart` » [`Leistungsarten (Kuerzel)`](../../tables/leistungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_FACHTAFELFAECHER_NIVEAU`**

:   `Niveau` » [`FachNiveaus (Kuerzel)`](../../tables/fachniveaus) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_FACHTAFELFAECHER_Q1`**

:   `Q1Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_FACHTAFELFAECHER_Q2`**

:   `Q2Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_FACHTAFELFAECHER_Q3`**

:   `Q3Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_FACHTAFELFAECHER_Q4`**

:   `Q4Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_FACHTAFELFAECHER_SCHWERPUNKT`**

:   `Schwerpunkt` » [`Fachschwerpunkte (Kuerzel)`](../../tables/fachschwerpunkte) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_FACHTAFELFAECHER_UNTERRICHT`**

:   `Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_FACHTAFELFAECHER_ZUKLASSE`**

:   `Mandant, Zusatzklasse` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 14 Indizes.

**`FK_FACHTAFELFAECHER_BILING`**

:   `Bilingual`

**`FK_FACHTAFELFAECHER_FACHSTATUS`**

:   `Fachstatus`

**`FK_FACHTAFELFAECHER_FACHTAFEL`**

:   `Mandant, Fachtafel`

**`FK_FACHTAFELFAECHER_HAUPTFACH`**

:   `Mandant, Hauptfach`

**`FK_FACHTAFELFAECHER_LART`**

:   `Leistungsart`

**`FK_FACHTAFELFAECHER_NIVEAU`**

:   `Niveau`

**`FK_FACHTAFELFAECHER_Q1`**

:   `Q1Bilingual`

**`FK_FACHTAFELFAECHER_Q2`**

:   `Q2Bilingual`

**`FK_FACHTAFELFAECHER_Q3`**

:   `Q3Bilingual`

**`FK_FACHTAFELFAECHER_Q4`**

:   `Q4Bilingual`

**`FK_FACHTAFELFAECHER_SCHWERPUNKT`**

:   `Schwerpunkt`

**`FK_FACHTAFELFAECHER_UNTERRICHT`**

:   `Unterrichtsart`

**`FK_FACHTAFELFAECHER_ZUKLASSE`**

:   `Mandant, Zusatzklasse`

**`PK_FACHTAFELFAECHER`**

:   `Mandant, ID`
