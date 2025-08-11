# Ansicht **WortersetzungenVerhaeltnisse**

## Abfrage

??? info "SQL"

    ``` sql
    SELECT 
        "ID",
        "BezeichnungOriginal",
        "BezeichnungAlternativ",
        case 
          When "ID" = 75 then 11
          When "ID" = 76 then 12
          When "ID" = 77 then 13
          When "ID" = 78 then 14
          When "ID" = 79 then 15
          When "ID" = 80 then 16
          When "ID" = 81 then 17
          When "ID" = 82 then 18
          When "ID" = 83 then 19
          When "ID" = 84 then 20
        else NULL
        end as "IDTransfer" 
      FROM "Wortersetzungen"
      WHERE ID Between 75 and 84
    ```

## Spalten

Diese Ansicht hat 4 Spalten.

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`BezeichnungOriginal`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`BezeichnungAlternativ`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`IDTransfer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)
