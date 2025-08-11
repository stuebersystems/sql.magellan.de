# Ansicht **MedizinDaten**

## Abfrage

??? info "SQL"

    ``` sql
    
      SELECT 
        S."Mandant", S."ID", S."EnbreaID", 1, S."Schueler", 'Sch?ler',    
        S."Kategorie", S."Art", S."Medikamente", S."Medikationen", 
        S."Bemerkung1", S."Bemerkung2", S."AblaufAm"
      FROM "SchuelerMedizinDaten" S
      UNION
      SELECT 
        L."Mandant", L."ID", L."EnbreaID", 2, L."Lehrer", 'Lehrer',    
        L."Kategorie", L."Art", L."Medikamente", L."Medikationen", 
        L."Bemerkung1", L."Bemerkung2", L."AblaufAm"
      FROM "LehrerMedizinDaten" L
      UNION
      SELECT 
        P."Mandant", P."ID", P."EnbreaID", 3, P."Person", 'Person',    
        P."Kategorie", P."Art", P."Medikamente", P."Medikationen", 
        P."Bemerkung1", P."Bemerkung2", P."AblaufAm"
      FROM "PersonenMedizinDaten" P
    ```

## Spalten

Diese Ansicht hat 13 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Typ`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`TypId`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`TypBezeichnung`**

:   [`CHAR(7)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Kategorie`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Art`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Medikamente`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Medikationen`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Bemerkung1`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Bemerkung2`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`AblaufAm`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)
