# Ansicht **LehrerLehraemter**

## Abfrage

??? info "SQL"

    ``` sql
    
    SELECT                                                                 
      T.*                                                                  
    FROM                                                                   
      "tblLehrerLehraemter" T                                              
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

## Spalten

Diese Ansicht hat 9 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Mandantenbezogene, eindeutige ID

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Lehramt`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Lehraemter](../../tables/lehraemter)

**`Typ`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    0 | Standard
    1 | Lehrbefähigung
    2 | Unterrichtserlaubnis
    3 | Unterrichtsauftrag
    4 | Unterrichtsbefugnis
    5 | Lehrbefähigung kleine Fakultas
    6 | Lehrbefähigung ohne Fakultas

**`Pruefungsbezug`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`JahrgangVon`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`JahrgangBis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Bemerkung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)
