# Tabelle **SchuelerKurswahlenDetails**

## Spalten

Diese Tabelle hat 26 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

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

**`Pflichtkurse`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`HJ1_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ2_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ3_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ4_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ5_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HJ6_Gewaehlt`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

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

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerKurswahlenDetails`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 7 Fremdschlüssel.

**`FK_SCHUELERKURSDETAILS_Q2`**

:   `Q2Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERKURSDETAILS_Q3`**

:   `Q3Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERKURSDETAILS_Q4`**

:   `Q4Bilingual` » [`Kurssprachen (Kuerzel)`](../../tables/kurssprachen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERKURSWAHLEND_ABI`**

:   `Mandant, Schueler` » [`SchuelerABI (Mandant, Schueler)`](../../tables/schuelerabi) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERKURSWAHLEND_FACH`**

:   `Fach, Mandant` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERKURSWAHLEND_FSTATUS`**

:   `Fachstatus` » [`Fachstati (Kuerzel)`](../../tables/fachstati) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

**`FK_SCHUELERKURSWAHLEND_UART`**

:   `Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

## Indizes

Diese Tabelle hat 9 Indizes.

**`FK_SCHUELERKURSDETAILS_Q1`**

:   `Q1Bilingual`

**`FK_SCHUELERKURSDETAILS_Q2`**

:   `Q2Bilingual`

**`FK_SCHUELERKURSDETAILS_Q3`**

:   `Q3Bilingual`

**`FK_SCHUELERKURSDETAILS_Q4`**

:   `Q4Bilingual`

**`FK_SCHUELERKURSWAHLEND_ABI`**

:   `Mandant, Schueler`

**`FK_SCHUELERKURSWAHLEND_FACH`**

:   `Mandant, Fach`

**`FK_SCHUELERKURSWAHLEND_FSTATUS`**

:   `Fachstatus`

**`FK_SCHUELERKURSWAHLEND_UART`**

:   `Unterrichtsart`

**`PK_SCHUELERKURSWAHLEND`**

:   `Mandant, ID`
