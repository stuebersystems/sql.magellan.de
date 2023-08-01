# Ansicht **AuswahlMedienAusleihe**

## Abfrage

??? info "SQL"

    ``` sql
    
    SELECT                                                                  
      T.*                                                                      
    FROM                                                                       
      "tblAuswahlMedienAusleihe" T                                            
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

**`Vorgang`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [MedienVorgaenge](../../tables/medienvorgaenge)

**`Ausleiher`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [MedienAusleiher](../../tables/medienausleiher)

**`Aktion`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)
