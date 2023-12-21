# Ansicht **AuswahlKlassenbuchKlassen**

## Abfrage

??? info "SQL"

    ``` sql
    
    SELECT                                                               
       T.*                                                                   
     FROM                                                                    
       "tblAuswahlKlassenbuchKlassen" T                                                  
     LEFT JOIN                                                               
       "tblBenutzer" B                                                       
     ON                                                                      
       B."Mandant" = T."Mandant" AND                                         
       B."Kennung" = T."Benutzer"                                            
     WHERE                                                                   
       B."Kennung" = USER
    ```

## Spalten

Diese Ansicht hat 6 Spalten.

**`Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`VonDatum`**

:   [`TIMESTAMP`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Zeitraum von

**`BisDatum`**

:   [`TIMESTAMP`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Zeitraum bis
