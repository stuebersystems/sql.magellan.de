# Table **tblLehrerLehraemter**

## Columns

This table contains 9 columns.

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

    Value | Description
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

## Primary key

This table has a primary key.

**`tblLehrerLehraemter`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_LEHRERLEHRAEMTER_LEHRAMT`**

:   `Lehramt` » [`Lehraemter (Kuerzel)`](../../tables/lehraemter) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_LEHRERLEHRAEMTER_LEHRER`**

:   `Lehrer, Mandant` » [`tblLehrer (ID, Mandant)`](../../tables/tbllehrer) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 4 indices.

**`FK_LEHRERLEHRAEMTER_BEZUG`**

:   `Pruefungsbezug`

**`FK_LEHRERLEHRAEMTER_LEHRAMT`**

:   `Lehramt`

**`FK_LEHRERLEHRAEMTER_LEHRER`**

:   `Mandant, Lehrer`

**`PK_LEHRERLEHRAEMTER`**

:   `Mandant, ID`
