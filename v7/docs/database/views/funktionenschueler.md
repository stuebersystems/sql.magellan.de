# View **FunktionenSchueler**

## Query

??? info "SQL"

    ``` sql
    
     SELECT
      "Mandant", "ID" AS "Schueler", "Funktion1" AS "Funktion"
    FROM
      "Schueler"
    WHERE
      NOT "Funktion1" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Schueler", "Funktion2" AS "Funktion"
    FROM
      "Schueler"
    WHERE
      NOT "Funktion2" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Schueler", "Funktion3" AS "Funktion"
    FROM
      "Schueler"
    WHERE
      NOT "Funktion3" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Schueler", "Funktion4" AS "Funktion"
    FROM
      "Schueler"
    WHERE
      NOT "Funktion4" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Schueler", "Funktion5" AS "Funktion"
    FROM
      "Schueler"
    WHERE
      NOT "Funktion5" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Schueler", "Funktion6" AS "Funktion"
    FROM
      "Schueler"
    WHERE
      NOT "Funktion6" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Schueler", "Funktion7" AS "Funktion"
    FROM
      "Schueler"
    WHERE
      NOT "Funktion7" IS NULL
    UNION SELECT
      "Mandant", "ID" AS "Schueler", "Funktion8" AS "Funktion"
    FROM
      "Schueler"
    WHERE
      NOT "Funktion8" IS NULL
    ```

## Columns

This view contains 3 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Funktion`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [SchuelerFunktionen](../../tables/schuelerfunktionen)
