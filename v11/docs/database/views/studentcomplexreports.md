# Ansicht **StudentComplexReports**

## Abfrage

??? info "SQL"

    ``` sql
    
      SELECT 
      SCR."Mandant", SCR."ID", SCR."PrevID", SCR."EnbreaID", SCR."StudentAchievement",
      SCR."Profile", SCR."Group", SCR."Entry",
      CASE
        WHEN not SCR."Entry" IS NULL THEN 0  
        WHEN not SCR."Group" IS NULL THEN 1
        ELSE 2    
      END AS "Type",   
      CASE
        WHEN not SCR."Entry" IS NULL THEN 1  
        WHEN not SCR."Group" IS NULL THEN AG."Configuration"
        ELSE AP."Configuration"    
      END AS "Configuration", 
      CASE
        WHEN not SCR."Entry" IS NULL THEN AE."Code"  
        WHEN not SCR."Group" IS NULL THEN AG."Code"
        ELSE AP."Code"    
      END AS "Code",
      CASE
        WHEN not SCR."Entry" IS NULL THEN AE."Name"  
        WHEN not SCR."Group" IS NULL THEN AG."Name"
        ELSE AP."Name"    
      END AS "Name",   
      CASE
        WHEN not SCR."Entry" IS NULL THEN AE."GradeSystem"  
        WHEN not SCR."Group" IS NULL THEN AG."GradeSystem"
        ELSE AP."GradeSystem"    
      END AS "GradeSystem",  
      SCR."Grade", SCR."Report", 
      AG."Position" AS "GroupPosition", 
      AE."Position" AS "EntryPosition"
      FROM "tblStudentComplexReports" SCR
      LEFT JOIN "AssessmentProfiles" AP
      ON  AP."Mandant" = SCR."Mandant"
      AND AP."ID" = SCR."Profile"
      LEFT JOIN "AssessmentGroups" AG
      ON  AG."Mandant" = SCR."Mandant"
      AND AG."Profile" = SCR."Profile"
      AND AG."ID" = SCR."Group"
      LEFT JOIN "AssessmentEntries" AE
      ON  AE."Mandant" = SCR."Mandant"
      AND AE."Profile" = SCR."Profile"
      AND AE."ID" = SCR."Entry"
    ```

## Spalten

Diese Ansicht hat 17 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Mandantenbezogene, eindeutige ID

**`PrevID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`StudentAchievement`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Profile`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Group`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Groups](../../tables/groups)

**`Entry`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Type`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Configuration`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Code`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Name`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`GradeSystem`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Grade`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Report`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`GroupPosition`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`EntryPosition`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)
