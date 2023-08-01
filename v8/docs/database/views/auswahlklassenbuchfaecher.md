# Ansicht **AuswahlKlassenbuchFaecher**

## Abfrage

??? info "SQL"

    ``` sql
    
    SELECT                                                               
       T.*                                                                   
     FROM                                                                    
       "tblAuswahlKlassenbuchFaecher" T                                                  
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

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`VonDatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Zeitraum von

**`BisDatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Zeitraum bis
