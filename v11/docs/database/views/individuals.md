# Ansicht **Individuals**

## Abfrage

??? info "SQL"

    ``` sql
    
      SELECT 
        M."Mandant", M."ID",  
        1 AS "Type", M."Vorname", M."Nachname", M."Strasse",
        M."Land", M."PLZ", M."Ort", M."Telefon", M."Email"
      FROM "Personen" M
      UNION
      SELECT 
        M."Mandant", M."ID", 
        2 AS "Type", M."Vorname", M."Nachname", M."Strasse",
        M."Land", M."PLZ", M."Ort", M."Telefon", M."Email"
      FROM "Lehrer" M
      UNION
      SELECT 
        M."Mandant", M."ID", 
        3 AS "Type", M."Vorname", M."Nachname", M."Strasse",
        M."Land", M."PLZ", M."Ort", M."Telefon", M."EMail"
      FROM "Schueler" M
      UNION
      SELECT 
        M."Mandant", M."ID",  
        4 AS "Type", M."Vorname", M."Nachname", M."Strasse",
        M."Land", M."PLZ", M."Ort", M."TelefonPrivat", M."Email"
      FROM "Sorgeberechtigte" M
    ```

## Spalten

Diese Ansicht hat 11 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Mandantenbezogene, eindeutige ID

**`Type`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Wert | Beschreibung
    - | -
    1 | Person
    2 | Lehrer
    3 | Schüler
    4 | Sorgeberechtigte

**`Firstname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Lastname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Street`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`State`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`ZipCode`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`City`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Phone`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Email`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)
