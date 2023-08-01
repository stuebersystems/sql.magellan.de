# Tabelle **SchuelerFoerderungen**

## Spalten

Diese Tabelle hat 15 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Behinderung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Behinderungsarten](../../tables/behinderungsarten)

**`Beeintraechtigung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Schwerpunkt1`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [FoerderSchwerpunkte](../../tables/foerderschwerpunkte)

**`Schwerpunkt2`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [FoerderSchwerpunkte](../../tables/foerderschwerpunkte)

**`Bedarf`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SopaedFoerderungen](../../tables/sopaedfoerderungen)

**`Ausgleich`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Gefoerdert`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Stunden1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Stunden2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Datensatzpositionierung

**`Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerFoerderungen`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 5 Fremdschlüssel.

**`FK_SCHUELERFOERDER_BEDARF`**

:   `Bedarf` » [`SopaedFoerderungen (Kuerzel)`](../../tables/sopaedfoerderungen) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

**`FK_SCHUELERFOERDER_BEHINDERUNG`**

:   `Behinderung` » [`Behinderungsarten (Kuerzel)`](../../tables/behinderungsarten) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

**`FK_SCHUELERFOERDER_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE NO ACTION` · `ON DELETE CASCADE`

**`FK_SCHUELERFOERDER_SCHWERPUNKT1`**

:   `Schwerpunkt1` » [`FoerderSchwerpunkte (Kuerzel)`](../../tables/foerderschwerpunkte) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

**`FK_SCHUELERFOERDER_SCHWERPUNKT2`**

:   `Schwerpunkt2` » [`FoerderSchwerpunkte (Kuerzel)`](../../tables/foerderschwerpunkte) · `ON UPDATE NO ACTION` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 7 Indizes.

**`FK_SCHUELERFOERDER_AUSGLEICH`**

:   `Ausgleich`

**`FK_SCHUELERFOERDER_BEDARF`**

:   `Bedarf`

**`FK_SCHUELERFOERDER_BEHINDERUNG`**

:   `Behinderung`

**`FK_SCHUELERFOERDER_SCHUELER`**

:   `Mandant, Schueler`

**`FK_SCHUELERFOERDER_SCHWERPUNKT1`**

:   `Schwerpunkt1`

**`FK_SCHUELERFOERDER_SCHWERPUNKT2`**

:   `Schwerpunkt2`

**`PK_SCHUELERFOERDERUNGEN`**

:   `Mandant, ID`
