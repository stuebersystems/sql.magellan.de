# View **AuswahlMedienAusleiher**

## Query

??? info "SQL"

    ``` sql
    
     SELECT                                                                  
      T.*                                                                      
    FROM                                                                       
      "tblAuswahlMedienAusleiher" T                                            
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

**`Ausleiher`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [MedienAusleiher](../../tables/medienausleiher)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Klassen](../../tables/klassen)
