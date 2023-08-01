# Table **SchuelerABIDetails**

## Columns

This table contains 47 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerABI](../../tables/schuelerabi)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerABI](../../tables/schuelerabi)

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Fachstatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachstati](../../tables/fachstati)

**`Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`Niveau`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [FachNiveaus](../../tables/fachniveaus)

**`HJ11_1_Punkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`HJ11_1_Eingebracht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Nicht eingebracht
    1 | Eingebracht
    2 | Gesperrt
    3 | Nicht drucken

**`HJ11_2_Punkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`HJ11_2_Eingebracht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Nicht eingebracht
    1 | Eingebracht
    2 | Gesperrt
    3 | Nicht drucken

**`HJ12_1_Punkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`HJ12_1_Eingebracht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Nicht eingebracht
    1 | Eingebracht
    2 | Gesperrt
    3 | Nicht drucken

**`HJ12_2_Punkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`HJ12_2_Eingebracht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Nicht eingebracht
    1 | Eingebracht
    2 | Gesperrt
    3 | Nicht drucken

**`HJ13_1_Punkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`HJ13_1_Eingebracht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Nicht eingebracht
    1 | Eingebracht
    2 | Gesperrt
    3 | Nicht drucken

**`HJ13_2_Punkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`HJ13_2_Eingebracht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Value | Description
    - | -
    0 | Nicht eingebracht
    1 | Eingebracht
    2 | Gesperrt
    3 | Nicht drucken

**`Summe`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Summe2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Faktor`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Q1Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Q2Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Q3Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Q4Bilingual`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Kurssprachen](../../tables/kurssprachen)

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`HJ1_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`HJ2_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`HJ3_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`HJ4_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`HJ5_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`HJ6_Muendlich`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`HJ1_Leistungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Leistungsarten](../../tables/leistungsarten)

**`HJ2_Leistungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Leistungsarten](../../tables/leistungsarten)

**`HJ3_Leistungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Leistungsarten](../../tables/leistungsarten)

**`HJ4_Leistungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Leistungsarten](../../tables/leistungsarten)

**`HJ5_Leistungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Leistungsarten](../../tables/leistungsarten)

**`HJ6_Leistungsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Leistungsarten](../../tables/leistungsarten)

**`HJ1_Bestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    P | Bestanden
    F | Nicht bestanden
    N | Nicht belegt

**`HJ2_Bestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    P | Bestanden
    F | Nicht bestanden
    N | Nicht belegt

**`HJ3_Bestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    P | Bestanden
    F | Nicht bestanden
    N | Nicht belegt

**`HJ4_Bestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    P | Bestanden
    F | Nicht bestanden
    N | Nicht belegt

**`HJ5_Bestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    P | Bestanden
    F | Nicht bestanden
    N | Nicht belegt

**`HJ6_Bestanden`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    P | Bestanden
    F | Nicht bestanden
    N | Nicht belegt

## Primary key

This table has a primary key.

**`SchuelerABIDetails`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_SCHUELERABIDETAILS_Q2`**

:   `Q2Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERABIDETAILS_Q3`**

:   `Q3Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERABIDETAILS_Q4`**

:   `Q4Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERABID_FACH`**

:   `Fach, Mandant` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERABID_HJ11_1`**

:   `HJ11_1_Punkte, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERABID_HJ11_2`**

:   `HJ11_2_Punkte, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERABID_HJ12_1`**

:   `HJ12_1_Punkte, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERABID_HJ12_2`**

:   `HJ12_2_Punkte, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERABID_HJ13_1`**

:   `HJ13_1_Punkte, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERABID_HJ13_2`**

:   `HJ13_2_Punkte, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERABID_LART_HJ1`**

:   `HJ1_Leistungsart` » [`Leistungsarten (Kuerzel)`](../../tables/leistungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERABID_LART_HJ2`**

:   `HJ2_Leistungsart` » [`Leistungsarten (Kuerzel)`](../../tables/leistungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERABID_LART_HJ3`**

:   `HJ3_Leistungsart` » [`Leistungsarten (Kuerzel)`](../../tables/leistungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERABID_LART_HJ4`**

:   `HJ4_Leistungsart` » [`Leistungsarten (Kuerzel)`](../../tables/leistungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERABID_LART_HJ5`**

:   `HJ5_Leistungsart` » [`Leistungsarten (Kuerzel)`](../../tables/leistungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERABID_LART_HJ6`**

:   `HJ6_Leistungsart` » [`Leistungsarten (Kuerzel)`](../../tables/leistungsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERABID_NIVEAU`**

:   `Niveau` » [`FachNiveaus (Kuerzel)`](../../tables/fachniveaus) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERABID_UNTERRICHTSART`**

:   `Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERBBSD_ABI`**

:   `Mandant, Schueler` » [`SchuelerABI (Mandant, Schueler)`](../../tables/schuelerabi) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 21 indices.

**`FK_SCHUELERABIDETAILS_Q1`**

:   `Q1Bilingual`

**`FK_SCHUELERABIDETAILS_Q2`**

:   `Q2Bilingual`

**`FK_SCHUELERABIDETAILS_Q3`**

:   `Q3Bilingual`

**`FK_SCHUELERABIDETAILS_Q4`**

:   `Q4Bilingual`

**`FK_SCHUELERABID_FACH`**

:   `Mandant, Fach`

**`FK_SCHUELERABID_HJ11_1`**

:   `Mandant, HJ11_1_Punkte`

**`FK_SCHUELERABID_HJ11_2`**

:   `Mandant, HJ11_2_Punkte`

**`FK_SCHUELERABID_HJ12_1`**

:   `Mandant, HJ12_1_Punkte`

**`FK_SCHUELERABID_HJ12_2`**

:   `Mandant, HJ12_2_Punkte`

**`FK_SCHUELERABID_HJ13_1`**

:   `Mandant, HJ13_1_Punkte`

**`FK_SCHUELERABID_HJ13_2`**

:   `Mandant, HJ13_2_Punkte`

**`FK_SCHUELERABID_LART_HJ1`**

:   `HJ1_Leistungsart`

**`FK_SCHUELERABID_LART_HJ2`**

:   `HJ2_Leistungsart`

**`FK_SCHUELERABID_LART_HJ3`**

:   `HJ3_Leistungsart`

**`FK_SCHUELERABID_LART_HJ4`**

:   `HJ4_Leistungsart`

**`FK_SCHUELERABID_LART_HJ5`**

:   `HJ5_Leistungsart`

**`FK_SCHUELERABID_LART_HJ6`**

:   `HJ6_Leistungsart`

**`FK_SCHUELERABID_NIVEAU`**

:   `Niveau`

**`FK_SCHUELERABID_UNTERRICHTSART`**

:   `Unterrichtsart`

**`FK_SCHUELERBBSD_ABI`**

:   `Mandant, Schueler`

**`PK_SCHUELERABIDETAILS`**

:   `Mandant, ID`
