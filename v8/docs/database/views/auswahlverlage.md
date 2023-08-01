# Ansicht **AuswahlVerlage**

## Abfrage

??? info "SQL"

    ``` sql
    
     SELECT
      T.*
    FROM
      "tblAuswahlVerlage" T
    LEFT JOIN
      "tblBenutzer" B
    ON
      B."Kennung" = T."Benutzer"
    WHERE
      B."Kennung" = USER
    ```

## Spalten

Diese Ansicht hat 2 Spalten.

**`Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Verlag`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Verlage](../../tables/verlage)
