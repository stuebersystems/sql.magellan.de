# View **MedizinAkten**

## Query

??? info "SQL"

    ``` sql
    
      SELECT 
        S."Mandant",S."ID", S."EnbreaID", 1, S."Schueler", 'Sch?ler', 
        S."Datum", S."Behandlung", S."Medikationen", S."Bemerkung"
      FROM "SchuelerMedizinAkten" S
      UNION
      SELECT 
        L."Mandant", L."ID", L."EnbreaID", 2, L."Lehrer", 'Lehrer',
        L."Datum", L."Behandlung", L."Medikationen", L."Bemerkung"
      FROM "LehrerMedizinAkten" L
      UNION
      SELECT 
        P."Mandant", P."ID", P."EnbreaID", 3, P."Person", 'Person',    
        P."Datum", P."Behandlung", P."Medikationen", P."Bemerkung"
      FROM "PersonenMedizinAkten" P
    ```

## Columns

This view contains 10 columns.

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

**`Datum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Behandlung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Medikationen`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)
