# Ansicht **ABIPruefungsfaecherSchriftlich**

## Abfrage

??? info "SQL"

    ``` sql
    
      SELECT
        SA."Mandant" || '.' ||  SA."Schueler" || '.' || S."Klasse" || '.' || S."Zeitraum" || '1' AS "ID",  
        SA."Mandant",     
        SA."Schueler",
        S."Klasse",
        S."Zeitraum",   
        S."Vorname",
        S."Vorname2",
        S."Namenszusatz",
        S."Nachname",          
        S."Geschlecht",
        S."Geburtsdatum",
        K."Notenart",
        SA."Pruefungsfach1" AS "Fach",
        1 AS "PF",
        SA."Jahrgang",
        SA."PruefungSchriftlich1Pruefer1",
        SA."PruefungSchriftlich1Pruefer2",
        SA."PruefungSchriftlich1",
        SAD."Lehrer",
        SAD."Unterrichtsart",
        SAD."Fachstatus",
        SAD."Summe2"    
      FROM "SchuelerABI" SA
      LEFT JOIN "SchuelerAnsicht" S
      ON  S."Mandant" = SA."Mandant"
      AND S.ID = SA."Schueler"
      AND S."Gewechselt" <> 'J'
      LEFT JOIN "Klassen" K
      ON  K."Mandant" = S."Mandant" 
      AND K."ID" = S."Klasse"
      LEFT JOIN "SchuelerABIDetails" SAD
      ON  SAD."Mandant" = SA."Mandant" 
      AND SAD."Schueler" = SA."Schueler"
      AND SAD."Fach" = SA."Pruefungsfach1"      
      UNION 
      SELECT
        SA."Mandant" || '.' ||  SA."Schueler" || '.' || S."Klasse" || '.' || S."Zeitraum" || '2' AS "ID",
        SA."Mandant", 
        SA."Schueler",
        S."Klasse",
        S."Zeitraum",   
        S."Vorname",
        S."Vorname2",
        S."Namenszusatz",
        S."Nachname",          
        S."Geschlecht",
        S."Geburtsdatum",
        K."Notenart",
        SA."Pruefungsfach2" AS "Fach",
        2 AS "PF",
        SA."Jahrgang",
        SA."PruefungSchriftlich2Pruefer1",
        SA."PruefungSchriftlich2Pruefer2",
        SA."PruefungSchriftlich2",
        SAD."Lehrer",
        SAD."Unterrichtsart",
        SAD."Fachstatus",
        SAD."Summe2"        
      FROM "SchuelerABI" SA
      LEFT JOIN "SchuelerAnsicht" S
      ON  S."Mandant" = SA."Mandant"
      AND S.ID = SA."Schueler"
      AND S."Gewechselt" <> 'J'
      LEFT JOIN "Klassen" K
      ON  K."Mandant" = S."Mandant" 
      AND K."ID" = S."Klasse"
      LEFT JOIN "SchuelerABIDetails" SAD
      ON  SAD."Mandant" = SA."Mandant" 
      AND SAD."Schueler" = SA."Schueler"
      AND SAD."Fach" = SA."Pruefungsfach2"     
      UNION 
      SELECT
        SA."Mandant" || '.' ||  SA."Schueler" || '.' || S."Klasse" || '.' || S."Zeitraum" || '3' AS "ID",
        SA."Mandant", 
        SA."Schueler",
        S."Klasse",
        S."Zeitraum",   
        S."Vorname",
        S."Vorname2",
        S."Namenszusatz",
        S."Nachname",          
        S."Geschlecht",
        S."Geburtsdatum",
        K."Notenart",
        SA."Pruefungsfach3" AS "Fach",
        3 AS "PF",
        SA."Jahrgang",
        SA."PruefungSchriftlich3Pruefer1",
        SA."PruefungSchriftlich3Pruefer2",
        SA."PruefungSchriftlich3",
        SAD."Lehrer",
        SAD."Unterrichtsart",
        SAD."Fachstatus",
        SAD."Summe2"        
      FROM "SchuelerABI" SA
      LEFT JOIN "SchuelerAnsicht" S
      ON  S."Mandant" = SA."Mandant"
      AND S.ID = SA."Schueler"
      AND S."Gewechselt" <> 'J'
      LEFT JOIN "Klassen" K
      ON  K."Mandant" = S."Mandant" 
      AND K."ID" = S."Klasse"
      LEFT JOIN "SchuelerABIDetails" SAD
      ON  SAD."Mandant" = SA."Mandant" 
      AND SAD."Schueler" = SA."Schueler"
      AND SAD."Fach" = SA."Pruefungsfach3"    
      UNION
      SELECT
        SA."Mandant" || '.' ||  SA."Schueler" || '.' || S."Klasse" || '.' || S."Zeitraum" || '4' AS "ID",
        SA."Mandant", 
        SA."Schueler",
        S."Klasse",
        S."Zeitraum",   
        S."Vorname",
        S."Vorname2",
        S."Namenszusatz",
        S."Nachname",          
        S."Geschlecht",
        S."Geburtsdatum",
        K."Notenart",
        SA."Pruefungsfach4" AS "Fach",
        4 AS "PF",
        SA."Jahrgang",
        SA."PruefungSchriftlich4Pruefer1",
        SA."PruefungSchriftlich4Pruefer2",
        SA."PruefungSchriftlich4",
        SAD."Lehrer",
        SAD."Unterrichtsart",
        SAD."Fachstatus",
        SAD."Summe2"        
      FROM "SchuelerABI" SA
      LEFT JOIN "SchuelerAnsicht" S
      ON  S."Mandant" = SA."Mandant"
      AND S.ID = SA."Schueler"
      AND S."Gewechselt" <> 'J'
      LEFT JOIN "Klassen" K
      ON  K."Mandant" = S."Mandant" 
      AND K."ID" = S."Klasse"
      LEFT JOIN "SchuelerABIDetails" SAD
      ON  SAD."Mandant" = SA."Mandant" 
      AND SAD."Schueler" = SA."Schueler"
      AND SAD."Fach" = SA."Pruefungsfach4"
    ```

## Spalten

Diese Ansicht hat 22 Spalten.

**`ID`**

:   [`VARCHAR(48)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Mandantenbezogene, eindeutige ID

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Zeitraum`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Zeitraeume](../../tables/zeitraeume)

**`Vorname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Vorname2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Namenszusatz`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Nachname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Geschlecht`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Wert | Beschreibung
    - | -
    W | Weiblich
    M | Weiblich
    D | Divers

**`Geburtsdatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Notenart`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

**`PF`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Jahrgang`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`NotePruefer1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`NotePruefer2`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Note`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Lehrer`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [tblLehrer](../../tables/tbllehrer)

**`Unterrichtsart`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Unterrichtsarten](../../tables/unterrichtsarten)

**`Fachstatus`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Fachstati](../../tables/fachstati)

**`Summe2`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)
