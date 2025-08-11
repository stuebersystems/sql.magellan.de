# Tabelle **SchuelerSPFDetails**

## Spalten

Diese Tabelle hat 10 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerSPF](../../tables/schuelerspf)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerSPF](../../tables/schuelerspf)

**`Sportfest`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Verweis auf Tabelle [SchuelerSPF](../../tables/schuelerspf)

**`Disziplin`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Zeit`**

:   [`TIME`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Weite`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Punkte`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Merkmal`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerSPFDetails`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_SCHUELERSPFD_SPORTFEST`**

:   `Mandant, Schueler, Sportfest` » [`SchuelerSPF (Mandant, Schueler, Sportfest)`](../../tables/schuelerspf) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_SCHUELERSPFD_DISZIPLIN`**

:   `Disziplin, Mandant` » [`Disziplinen (Kuerzel, Mandant)`](../../tables/disziplinen) · `ON UPDATE CASCADE` · `ON DELETE RESTRICT`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_SCHUELERSPFD_DISZIPLIN`**

:   `Mandant, Disziplin`

**`FK_SCHUELERSPFD_SPORTFEST`**

:   `Mandant, Schueler, Sportfest`

**`PK_SCHUELERSPFDETAILS`**

:   `Mandant, ID`
