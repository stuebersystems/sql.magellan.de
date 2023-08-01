# Ansicht **FunktionenSorgebe**

## Abfrage

??? info "SQL"

    ``` sql
    
     SELECT
      "Mandant", "ID" AS "Sorgebe", "Funktion1" AS "Funktion"
    FROM
      "Sorgeberechtigte"
    WHERE
      NOT "Funktion1" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Sorgebe", "Funktion2" AS "Funktion"
    FROM
      "Sorgeberechtigte"
    WHERE
      NOT "Funktion2" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Sorgebe", "Funktion3" AS "Funktion"
    FROM
      "Sorgeberechtigte"
    WHERE
      NOT "Funktion3" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Sorgebe", "Funktion4" AS "Funktion"
    FROM
      "Sorgeberechtigte"
    WHERE
      NOT "Funktion4" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Sorgebe", "Funktion5" AS "Funktion"
    FROM
      "Sorgeberechtigte"
    WHERE
      NOT "Funktion5" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Sorgebe", "Funktion6" AS "Funktion"
    FROM
      "Sorgeberechtigte"
    WHERE
      NOT "Funktion6" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Sorgebe", "Funktion7" AS "Funktion"
    FROM
      "Sorgeberechtigte"
    WHERE
      NOT "Funktion7" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Sorgebe", "Funktion8" AS "Funktion"
    FROM
      "Sorgeberechtigte"
    WHERE
      NOT "Funktion8" IS NULL
    ```

## Spalten

Diese Ansicht hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Sorgebe`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Sorgeberechtigte](../../tables/sorgeberechtigte)

**`Funktion`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SorgbeFunktionen](../../tables/sorgbefunktionen)
