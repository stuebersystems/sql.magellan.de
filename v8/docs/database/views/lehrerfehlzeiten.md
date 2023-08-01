# View **LehrerFehlzeiten**

## Query

??? info "SQL"

    ``` sql
    
    SELECT                                                                 
      T."Mandant",
      T.ID,
      T."Lehrer",
      T."Von",
      T."Bis",
      T."Stunden",
      T."Unterrichtstage",
      T."Fehltage", 
      T."Grund",
      T."Voranfrage",
      T."Bemerkung"                                                                  
    FROM                                                                   
      "tblLehrerFehlzeiten" T                                              
    LEFT JOIN                                                              
      "tblBenutzer" B                                                      
    ON                                                                     
      B."Mandant" = T."Mandant"                                            
    WHERE                                                                  
      B."Kennung" = USER                                                   
    AND
    ((B."Lehrer" = T."Lehrer") OR (B."Gruppe1" = 0 OR B."Gruppe1" = 1 OR
                                     B."Gruppe1" = 4 OR B."Gruppe1" = 5 OR
                                     B."Gruppe1" = 9))
    ```

## Columns

This view contains 11 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Mandantenbezogene, eindeutige ID

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Von`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Bis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Stunden`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Unterrichtstage`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Fehltage`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Grund`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Voranfrage`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    N | Nein
    J | Ja

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)
