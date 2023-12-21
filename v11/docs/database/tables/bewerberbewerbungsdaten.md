# Tabelle **BewerberBewerbungsdaten**

## Spalten

Diese Tabelle hat 65 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Klassenstufe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Klassenstufen](../../tables/klassenstufen)

**`Empfehlung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bewerbungsempfehlungen](../../tables/bewerbungsempfehlungen)

**`Schulwunsch2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Schulwunsch3`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schulen](../../tables/schulen)

**`Haertefall`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Haertefaelle](../../tables/haertefaelle)

**`BonusWartezeit`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Bonus für Wartezeit

**`BonusVorbildung`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Bonus für Vorbildung

**`BonusHaertefall`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Bonus für Härtefall

**`BonusSonstiges`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Sonstiger Bonus

**`BonusGesamt`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Gesamtbonus

**`HFNoteDeutsch`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Note Deutsch

**`HFNoteMathematik`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Note Mathematik

**`HFNoteFS1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Note Fremdsprache 1

**`HFNoteFS2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Note Fremdsprache 2

**`HFNoteFS3`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Note Fremdsprache 3

**`HFNoteFach1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Note sonstiges Fach 1

**`HFNoteFach2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Note sonstiges Fach 2

**`HFNoteFach3`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Note sonstiges Fach 3

**`HFDurchschnitt`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Durchschnitt

**`HFMitBonus`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Gesamtbonus bei Hauptfachdurchschnitt berücksichtigen

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`HFEndDurchschnitt`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Hauptfach Durchschnitt für das Bewerberverfahren

**`GesamtDurchschnitt`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Zeugnisdurchschnitt

**`GesamtDurchschnittMitBonus`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Gesamtbonus bei Zeugnisdurchschnitt berücksichtigen

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`GesamtEndDurchschnitt`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Zeugnisdurchschnitt für das Bewerberverfahren

**`GesamtPunkte`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

    Gesamtpunktzahl für das Bewerberverfahren

**`Profilfach1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Profilfach1Gewicht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Profilfach1Note1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach1Note2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Profilfach2Gewicht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Profilfach2Note1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach2Note2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach3`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Profilfach3Gewicht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Profilfach3Note1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach3Note2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach4`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Profilfach4Gewicht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Profilfach4Note1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach4Note2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach5`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Profilfach5Gewicht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Profilfach5Note1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach5Note2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach6`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`Profilfach6Gewicht`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Profilfach6Note1`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Profilfach6Note2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`ProfilfachSumme`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Kompetenz`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Test`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`GesamtDurchschnittPunkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`ProfilPunkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`KompetenzPunkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`TestPunkte`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`PunkteRanking`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`ExtPruefungFSP`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | bereits absolviert
    1 | angestrebt

**`QuereinsteigerFSP2`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `DEFAULT 'N'`

    Wert | Beschreibung
    - | -
    N | Nein
    J | Ja

**`Feststellungspruefung`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`QVermerk`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Aufnahmehalbjahr`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`BewerberBewerbungsdaten`**

:   `Mandant, Schueler`

## Fremdschlüssel

Diese Tabelle hat 12 Fremdschlüssel.

**`FK_BBD_HAERTEFALL`**

:   `Haertefall` » [`Haertefaelle (Kuerzel)`](../../tables/haertefaelle) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_KLASSENSTUFE`**

:   `Klassenstufe` » [`Klassenstufen (Kuerzel)`](../../tables/klassenstufen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_PROFILFACH1`**

:   `Mandant, Profilfach1` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_PROFILFACH2`**

:   `Mandant, Profilfach2` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_PROFILFACH3`**

:   `Mandant, Profilfach3` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_PROFILFACH4`**

:   `Mandant, Profilfach4` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_PROFILFACH5`**

:   `Mandant, Profilfach5` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_PROFILFACH6`**

:   `Mandant, Profilfach6` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_SCHULWUNSCH2`**

:   `Schulwunsch2` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BBD_SCHULWUNSCH3`**

:   `Schulwunsch3` » [`Schulen (ID)`](../../tables/schulen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

**`FK_BEWERBERBEWERBUNGSDATEN`**

:   `Mandant, Schueler` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_BBD_EMPFEHLUNG`**

:   `Empfehlung` » [`Bewerbungsempfehlungen (Kuerzel)`](../../tables/bewerbungsempfehlungen) · `ON UPDATE RESTRICT` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 13 Indizes.

**`FK_BBD_EMPFEHLUNG`**

:   `Empfehlung`

**`FK_BBD_HAERTEFALL`**

:   `Haertefall`

**`FK_BBD_KLASSENSTUFE`**

:   `Klassenstufe`

**`FK_BBD_PROFILFACH1`**

:   `Mandant, Profilfach1`

**`FK_BBD_PROFILFACH2`**

:   `Mandant, Profilfach2`

**`FK_BBD_PROFILFACH3`**

:   `Mandant, Profilfach3`

**`FK_BBD_PROFILFACH4`**

:   `Mandant, Profilfach4`

**`FK_BBD_PROFILFACH5`**

:   `Mandant, Profilfach5`

**`FK_BBD_PROFILFACH6`**

:   `Mandant, Profilfach6`

**`FK_BBD_SCHULWUNSCH2`**

:   `Schulwunsch2`

**`FK_BBD_SCHULWUNSCH3`**

:   `Schulwunsch3`

**`FK_BEWERBERBEWERBUNGSDATEN`**

:   `Mandant, Schueler`

**`PK_BEWERBUNGSDATEN`**

:   `Mandant, Schueler`
