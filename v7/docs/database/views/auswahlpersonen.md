# View **AuswahlPersonen**

## Query

??? info "SQL"

    ``` sql
    
     SELECT                                  
      T.*                                      
    FROM                                       
      "tblAuswahlPersonen" T                   
    LEFT JOIN                                  
      "tblBenutzer" B                          
    ON                                         
      B."Mandant" = T."Mandant" AND            
      B."Kennung" = T."Benutzer"               
    WHERE                                      
      B."Kennung" = USER
    ```

## Columns

This view contains 4 columns.

**`Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Person`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Personen](../../tables/personen)
