# Ansicht **BenutzerLogbuch**

## Abfrage

??? info "SQL"

    ``` sql
    
    SELECT
      T.ID,
      T."Benutzer",
      T."Aktion",
      T."EintragDatum",
      T."EintragUhrzeit"
    FROM
      "tblBenutzerLogbuch" T
    WHERE
      ("Benutzer" = USER) or (USER = 'SYSDBA') or (USER = 'DBADMIN')
    ```

## Spalten

Diese Ansicht hat 5 Spalten.

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Eindeutige ID

**`Benutzer`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Aktion`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EintragDatum`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`EintragUhrzeit`**

:   [`TIME`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)
