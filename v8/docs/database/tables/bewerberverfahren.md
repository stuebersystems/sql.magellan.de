# Table **BewerberVerfahren**

## Columns

This table contains 11 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`BrueckenKurseDE`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`BrueckenKurseMA`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`BrueckenKurseEN`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EinschaetzungLehrer`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Value | Description
    - | -
    3 | A
    2 | B
    1 | C

**`EinschaetzungBewerber`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Value | Description
    - | -
    3 | A
    2 | B
    1 | C

**`BewerberStatus`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Value | Description
    - | -
    0 | Auf Warteliste
    1 | Angenommen für Bildungsziel 1
    2 | Angenommen für Bildungsziel 2
    3 | Angenommen für Bildungsziel 3
    4 | Nicht angenommen
    5 | Angenommen für Bildungsziel 4
    6 | Beratungstest
    7 | Beratungsgespräch
    8 | Nicht zum Gespräch\/Testerschienen
    9 | Aufnahmebescheid
    10 | Zusage nicht zurück
    11 | Abgemeldet
    12 | Rückmeldung
    13 | Ablehnungsbescheid

**`VerfahrenStatus`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Termininfo`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

## Primary key

This table has a primary key.

**`BewerberVerfahren`**

:   `Mandant, Schueler`

## Indices

This table has one index.

**`PK_BEWERBERVERFAHREN`**

:   `Mandant, Schueler`
