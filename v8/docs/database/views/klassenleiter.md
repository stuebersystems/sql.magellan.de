# Ansicht **Klassenleiter**

## Abfrage

??? info "SQL"

    ``` sql
    
     SELECT
      "Mandant", "Klasse", "Zeitraum", "Klassenleiter1" AS "Leiter"
    FROM
      "KlassenZeitraeume"
    WHERE
      NOT "Klassenleiter1" IS NULL
    UNION SELECT
      "Mandant", "Klasse", "Zeitraum", "Klassenleiter2" AS "Leiter"
    FROM
      "KlassenZeitraeume"
    WHERE
      NOT "Klassenleiter2" IS NULL
    ```

## Spalten

Diese Ansicht hat 4 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Leiter`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)
