# Ansicht **GroupMembers**

## Abfrage

??? info "SQL"

    ``` sql
    
      SELECT 
        GM."Mandant", GM."ID", GM."EnbreaID", 
        GM."Group", G."Code", G."Name",
        GM."MemberID", GM."MemberType", M."Vorname", M."Nachname", M."Strasse",
        M."Land", M."PLZ", M."Ort", M."Telefon", M."Email",
        GM."StartedAt", GM."FinishedAt", GM."Contribution", GM."ContributionPaidOn",
        GM."Function1", GM."Function2"
      FROM "tblGroupMembers" GM
      LEFT JOIN "Groups" G
      ON  G."Mandant" = GM."Mandant"
      AND G."ID" = GM."Group"
      LEFT JOIN "Personen" M
      ON  M."Mandant" = GM."Mandant"
      AND M."ID" = GM."MemberID"
      WHERE
        GM."MemberType" = 1
      UNION
      SELECT 
        GM."Mandant", GM."ID", GM."EnbreaID", 
        GM."Group", G."Code", G."Name",
        GM."MemberID", GM."MemberType", M."Vorname", M."Nachname", M."Strasse",
        M."Land", M."PLZ", M."Ort", M."Telefon", M."Email",
        GM."StartedAt", GM."FinishedAt", GM."Contribution", GM."ContributionPaidOn",
        GM."Function1", GM."Function2"
      FROM "tblGroupMembers" GM
      LEFT JOIN "Groups" G
      ON  G."Mandant" = GM."Mandant"
      AND G."ID" = GM."Group"
      LEFT JOIN "Lehrer" M
      ON  M."Mandant" = GM."Mandant"
      AND M."ID" = GM."MemberID"
      WHERE
        GM."MemberType" = 2  
      UNION
      SELECT 
        GM."Mandant", GM."ID", GM."EnbreaID", 
        GM."Group", G."Code", G."Name",
        GM."MemberID", GM."MemberType", M."Vorname", M."Nachname", M."Strasse",
        M."Land", M."PLZ", M."Ort", M."Telefon", M."EMail",
        GM."StartedAt", GM."FinishedAt", GM."Contribution", GM."ContributionPaidOn",
        GM."Function1", GM."Function2"
      FROM "tblGroupMembers" GM
      LEFT JOIN "Groups" G
      ON  G."Mandant" = GM."Mandant"
      AND G."ID" = GM."Group"
      LEFT JOIN "Schueler" M
      ON  M."Mandant" = GM."Mandant"
      AND M."ID" = GM."MemberID"
      WHERE
        GM."MemberType" = 3      
      UNION
      SELECT 
        GM."Mandant", GM."ID", GM."EnbreaID", 
        GM."Group", G."Code", G."Name",
        GM."MemberID", GM."MemberType", M."Vorname", M."Nachname", M."Strasse",
        M."Land", M."PLZ", M."Ort", M."TelefonPrivat", M."Email",
        GM."StartedAt", GM."FinishedAt", GM."Contribution", GM."ContributionPaidOn",
        GM."Function1", GM."Function2"
      FROM "tblGroupMembers" GM
      LEFT JOIN "Groups" G
      ON  G."Mandant" = GM."Mandant"
      AND G."ID" = GM."Group"
      LEFT JOIN "Sorgeberechtigte" M
      ON  M."Mandant" = GM."Mandant"
      AND M."ID" = GM."MemberID"
      WHERE
        GM."MemberType" = 4
    ```

## Spalten

Diese Ansicht hat 22 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Group`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Groups](../../tables/groups)

**`GroupCode`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`GroupName`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MemberID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`MemberType`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`MemberFirstname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MemberLastname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MemberStreet`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MemberState`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MemberZipCode`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MemberCity`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MemberPhone`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`MemberEmail`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`StartedAt`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`FinishedAt`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Contribution`**

:   [`NUMERIC(?, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`ContributionPaidOn`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

**`Function1`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Function2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)
