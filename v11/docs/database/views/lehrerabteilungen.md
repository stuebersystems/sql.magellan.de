# Ansicht **LehrerAbteilungen**

## Abfrage

??? info "SQL"

    ``` sql
    
     SELECT
      "Mandant", "ID" AS "Lehrer", "Abteilung1" AS "Abteilung"
    FROM
     "Lehrer"
    WHERE
      NOT "Abteilung1" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Abteilung2" AS "Abteilung"
      FROM  "Lehrer"
      WHERE NOT "Abteilung2" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Abteilung3" AS "Abteilung"
      FROM "Lehrer"
      WHERE NOT "Abteilung3" IS NULL
    ```

## Spalten

Diese Ansicht hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Abteilung`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Abteilungen](../../tables/abteilungen)
