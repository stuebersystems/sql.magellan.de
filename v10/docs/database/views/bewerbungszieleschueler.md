# Ansicht **BewerbungszieleSchueler**

## Abfrage

??? info "SQL"

    ``` sql
    
     SELECT
        "Mandant", "ID" AS "Schueler", "Bewerbungsziel1" AS "Bewerbungsziel",
        "BewerberRangzahlZiel1" AS "Rangzahl"
      FROM
        "Schueler"
      WHERE
        NOT "Bewerbungsziel1" IS NULL
      UNION SELECT
        "Mandant", "ID" AS "Schueler", "Bewerbungsziel2" AS "Bewerbungsziel",
        "BewerberRangzahlZiel2" AS "Rangzahl"
      FROM
        "Schueler"
      WHERE
        NOT "Bewerbungsziel2" IS NULL
      UNION SELECT
        "Mandant", "ID" AS "Schueler", "Bewerbungsziel3" AS "Bewerbungsziel",
        "BewerberRangzahlZiel3" AS "Rangzahl"
      FROM
        "Schueler"
      WHERE
        NOT "Bewerbungsziel3" IS NULL
      UNION SELECT
        "Mandant", "ID" AS "Schueler", "Bewerbungsziel4" AS "Bewerbungsziel",
        "BewerberRangzahlZiel4" AS "Rangzahl"
      FROM
        "Schueler"
      WHERE
        NOT "Bewerbungsziel4" IS NULL
    ```

## Spalten

Diese Ansicht hat 4 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Bewerbungsziel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Bewerbungsziele](../../tables/bewerbungsziele)

**`Rangzahl`**

:   [`NUMERIC(?, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)
