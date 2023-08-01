# Ansicht **FunktionenLehrer**

## Abfrage

??? info "SQL"

    ``` sql
    
     SELECT
      "Mandant", "ID" AS "Lehrer", "Funktion1" AS "Funktion"
    FROM
      "Lehrer"
    WHERE
      NOT "Funktion1" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Funktion2" AS "Funktion"
      FROM "Lehrer"
      WHERE NOT "Funktion2" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Funktion3" AS "Funktion"
      FROM "Lehrer"
      WHERE NOT "Funktion3" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Funktion4" AS "Funktion"
       FROM "Lehrer"
      WHERE NOT "Funktion4" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Funktion5" AS "Funktion"
      FROM "Lehrer"
      WHERE NOT "Funktion5" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Funktion6" AS "Funktion"
      FROM "Lehrer"
      WHERE NOT "Funktion6" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Funktion7" AS "Funktion"
      FROM "Lehrer"
      WHERE NOT "Funktion7" IS NULL
    UNION
      SELECT "Mandant", "ID" AS "Lehrer", "Funktion8" AS "Funktion"
      FROM "Lehrer"
      WHERE NOT "Funktion8" IS NULL
    ```

## Spalten

Diese Ansicht hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Funktion`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [LehrerFunktionen](../../tables/lehrerfunktionen)
