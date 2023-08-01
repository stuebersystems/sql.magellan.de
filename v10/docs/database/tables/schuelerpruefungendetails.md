# Tabelle **SchuelerPruefungenDetails**

## Spalten

Diese Tabelle hat 30 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Noten](../../tables/noten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerPruefungen](../../tables/schuelerpruefungen)

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`ParentSPD`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [SchuelerPruefungenDetails](../../tables/schuelerpruefungendetails)

**`Fachstatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachstati](../../tables/fachstati)

**`Fachgruppe`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`HJ1_Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`HJ1_Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`HJ1_Note`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`HJ2_Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`HJ2_Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`HJ2_Note`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`HJ3_Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`HJ3_Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`HJ3_Note`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`VN_Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`VN_Berechnet`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`VN_Note`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`VN_NoteMarkiert`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`PR_Note1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`PR_Note2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`PR_Note3`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Noten](../../tables/noten)

**`EN_Unterrichtsart1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`EN_Note1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EN_Note1Markiert`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EN_Unterrichtsart2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`EN_Note2`**

:   [`NUMERIC(18, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerPruefungenDetails`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 21 Fremdschlüssel.

**`FK_SCHPRUEFDET_EN_UART1`**

:   `EN_Unterrichtsart1` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_EN_UART2`**

:   `EN_Unterrichtsart2` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_FACH`**

:   `Fach, Mandant` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_FACHSTATUS`**

:   `Fachstatus` » [`Fachstati (Kuerzel)`](../../tables/fachstati) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ1_LEHRER`**

:   `HJ1_Lehrer, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ1_NOTE`**

:   `HJ1_Note, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ1_UART`**

:   `HJ1_Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ2_LEHRER`**

:   `HJ2_Lehrer, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ2_NOTE`**

:   `HJ2_Note, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ2_UART`**

:   `HJ2_Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ3_LEHRER`**

:   `HJ3_Lehrer, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ3_NOTE`**

:   `HJ3_Note, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_HJ3_UART`**

:   `HJ3_Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_PARENTSPD`**

:   `Mandant, ParentSPD` » [`SchuelerPruefungenDetails (ID, Mandant)`](../../tables/schuelerpruefungendetails) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_PR_NOTE1`**

:   `Mandant, PR_Note1` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_PR_NOTE2`**

:   `Mandant, PR_Note2` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_PR_NOTE3`**

:   `Mandant, PR_Note3` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_SCHPRUEF`**

:   `Mandant, SchuelerZeitraumID` » [`SchuelerPruefungen (Mandant, SchuelerZeitraumID)`](../../tables/schuelerpruefungen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHPRUEFDET_VN_NOTE`**

:   `Mandant, VN_Note` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_VN_UART`**

:   `VN_Unterrichtsart` » [`Unterrichtsarten (Kuerzel)`](../../tables/unterrichtsarten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_SCHPRUEFDET_EN_NOTE1`**

:   `EN_Note1, Mandant` » [`Noten (ID, Mandant)`](../../tables/noten) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 22 Indizes.

**`FK_SCHPRUEFDET_EN_NOTE1`**

:   `Mandant, EN_Note1`

**`FK_SCHPRUEFDET_EN_UART1`**

:   `EN_Unterrichtsart1`

**`FK_SCHPRUEFDET_EN_UART2`**

:   `EN_Unterrichtsart2`

**`FK_SCHPRUEFDET_FACH`**

:   `Mandant, Fach`

**`FK_SCHPRUEFDET_FACHSTATUS`**

:   `Fachstatus`

**`FK_SCHPRUEFDET_HJ1_LEHRER`**

:   `Mandant, HJ1_Lehrer`

**`FK_SCHPRUEFDET_HJ1_NOTE`**

:   `Mandant, HJ1_Note`

**`FK_SCHPRUEFDET_HJ1_UART`**

:   `HJ1_Unterrichtsart`

**`FK_SCHPRUEFDET_HJ2_LEHRER`**

:   `Mandant, HJ2_Lehrer`

**`FK_SCHPRUEFDET_HJ2_NOTE`**

:   `Mandant, HJ2_Note`

**`FK_SCHPRUEFDET_HJ2_UART`**

:   `HJ2_Unterrichtsart`

**`FK_SCHPRUEFDET_HJ3_LEHRER`**

:   `Mandant, HJ3_Lehrer`

**`FK_SCHPRUEFDET_HJ3_NOTE`**

:   `Mandant, HJ3_Note`

**`FK_SCHPRUEFDET_HJ3_UART`**

:   `HJ3_Unterrichtsart`

**`FK_SCHPRUEFDET_PARENTSPD`**

:   `Mandant, ParentSPD`

**`FK_SCHPRUEFDET_PR_NOTE1`**

:   `Mandant, PR_Note1`

**`FK_SCHPRUEFDET_PR_NOTE2`**

:   `Mandant, PR_Note2`

**`FK_SCHPRUEFDET_PR_NOTE3`**

:   `Mandant, PR_Note3`

**`FK_SCHPRUEFDET_SCHPRUEF`**

:   `Mandant, SchuelerZeitraumID`

**`FK_SCHPRUEFDET_VN_NOTE`**

:   `Mandant, VN_Note`

**`FK_SCHPRUEFDET_VN_UART`**

:   `VN_Unterrichtsart`

**`PK_SCHUELERPRUEFUNGENDETAILS`**

:   `Mandant, ID`
