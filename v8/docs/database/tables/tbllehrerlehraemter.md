# Tabelle **tblLehrerLehraemter**

## Spalten

Diese Tabelle hat 9 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Lehramt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [Lehraemter](../../tables/lehraemter)

**`Typ`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Standard
    1 | Lehrbefähigung
    2 | Unterrichtserlaubnis
    3 | Unterrichtsauftrag
    4 | Unterrichtsbefugnis
    5 | Lehrbefähigung kleine Fakultas
    6 | Lehrbefähigung ohne Fakultas

**`Pruefungsbezug`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`JahrgangVon`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`JahrgangBis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Bemerkung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`tblLehrerLehraemter`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_LEHRERLEHRAEMTER_LEHRAMT`**

:   `Lehramt` » [`Lehraemter (Kuerzel)`](../../tables/lehraemter) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_LEHRERLEHRAEMTER_LEHRER`**

:   `Lehrer, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 4 Indizes.

**`FK_LEHRERLEHRAEMTER_BEZUG`**

:   `Pruefungsbezug`

**`FK_LEHRERLEHRAEMTER_LEHRAMT`**

:   `Lehramt`

**`FK_LEHRERLEHRAEMTER_LEHRER`**

:   `Mandant, Lehrer`

**`PK_LEHRERLEHRAEMTER`**

:   `Mandant, ID`
