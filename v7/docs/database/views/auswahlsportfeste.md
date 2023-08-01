# Ansicht **AuswahlSportfeste**

## Abfrage

??? info "SQL"

    ``` sql
    
     SELECT                                  
      T.*                                      
    FROM                                       
      "tblAuswahlSportfeste" T                 
    LEFT JOIN                                  
      "tblBenutzer" B                          
    ON                                         
      B."Mandant" = T."Mandant" AND            
      B."Kennung" = T."Benutzer"               
    WHERE                                      
      B."Kennung" = USER
    ```

## Spalten

Diese Ansicht hat 5 Spalten.

**`Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Sportfest`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Sportfeste](../../tables/sportfeste)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schueler](../../tables/schueler)
