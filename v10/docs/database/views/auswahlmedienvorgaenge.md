# View **AuswahlMedienVorgaenge**

## Query

??? info "SQL"

    ``` sql
    
     SELECT
      T.*
    FROM
      "tblAuswahlMedienVorgaenge" T
    LEFT JOIN
      "tblBenutzer" B
    ON
      B."Mandant" = T."Mandant" AND
      B."Kennung" = T."Benutzer"
    WHERE
      B."Kennung" = USER
    ```

## Columns

This view contains 3 columns.

**`Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Vorgang`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [MedienVorgaenge](../../tables/medienvorgaenge)
