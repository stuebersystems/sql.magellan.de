# Tabelle **SchuelerSchulen**

## Spalten

Diese Tabelle hat 17 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Schule`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Schulform`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchulformenHerkunft](../../tables/schulformenherkunft)

**`Schulart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchulartenHerkunft](../../tables/schulartenherkunft)

**`Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`LetzteKlasse`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Klassenleiter`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Abschluss`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Herkunft`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Unterlagen`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Herkunftsunterlagen](../../tables/herkunftsunterlagen)

**`Sprachfoerderung`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Laufbahn`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Einschulung in die Primarstufe
    1 | Übergang in die SEK I
    2 | Übergang in die SEK II
    3 | Übergang in BBS
    4 | Zuletzt besuchte Schule

**`Klassenstufe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Klassenstufen](../../tables/klassenstufen)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`SchuelerSchulen`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 7 Fremdschlüssel.

**`FK_SCHUELERS_SCHUELER`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_SCHUELERS_SCHULART`**

:   `Schulart` » [`SchulartenHerkunft (Kuerzel)`](../../tables/schulartenherkunft) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERS_SCHULE`**

:   `Schule` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_SCHUELERS_SCHULFORM`**

:   `Schulform` » [`SchulformenHerkunft (Kuerzel)`](../../tables/schulformenherkunft) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERS_STUFE`**

:   `Klassenstufe` » [`Klassenstufen (Kuerzel)`](../../tables/klassenstufen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERS_UNTERLAGEN`**

:   `Unterlagen` » [`Herkunftsunterlagen (Kuerzel)`](../../tables/herkunftsunterlagen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_SCHUELERS_HERKUNFT`**

:   `Herkunft` » [`Herkunftsarten (Kuerzel)`](../../tables/herkunftsarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 8 Indizes.

**`FK_SCHUELERS_HERKUNFT`**

:   `Herkunft`

**`FK_SCHUELERS_SCHUELER`**

:   `Mandant, Schueler`

**`FK_SCHUELERS_SCHULART`**

:   `Schulart`

**`FK_SCHUELERS_SCHULE`**

:   `Schule`

**`FK_SCHUELERS_SCHULFORM`**

:   `Schulform`

**`FK_SCHUELERS_STUFE`**

:   `Klassenstufe`

**`FK_SCHUELERS_UNTERLAGEN`**

:   `Unterlagen`

**`PK_SCHUELERSCHULEN`**

:   `Mandant, ID`
