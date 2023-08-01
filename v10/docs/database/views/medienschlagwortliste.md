# Ansicht **MedienSchlagwortliste**

## Abfrage

??? info "SQL"

    ``` sql
    
    SELECT
        MS."Mandant",
        MS."Medium",
        S."Bezeichnung"
    FROM
      "Schlagworte" S
    LEFT JOIN
      "MedienSchlagworte" MS
    ON
      MS."Mandant" = S."Mandant" AND
      MS."Schlagwort" = S."ID"
    ```

## Spalten

Diese Ansicht hat 3 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Medium`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Medien](../../tables/medien)

**`Schlagwort`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)
