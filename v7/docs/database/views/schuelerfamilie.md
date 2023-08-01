# View **SchuelerFamilie**

## Query

??? info "SQL"

    ``` sql
    
      SELECT DISTINCT
        SS."Mandant", SS."ID", 
        SS."Familiennr", SS."Verhaeltnis", SS."Sorgerecht", SS."Benachrichtigung", 
        SS."SeriendruckName1", SS."SeriendruckName2", SS."Briefempfaenger", 
        SS."Briefanrede", SS."TelefonPrioritaet", SS."Position", SS."Bemerkung",     
        SS."Schueler", S."Vorname", S."Nachname",
        SS."Person", 1, CAST('Person' AS VARCHAR(15)), P."Vorname", P."Nachname", P."Namenszusatz", 
        P."Anrede", P."Strasse", P."Adresszusatz", P."Land", P."PLZ", P."Ort", P."Ortsteil",
        P."Adressgebiet", P."Gemeinde", 
        P."Telefon", P."TelefonDienst", P."Mobil", P."Email",
        P."HeimatName1", P."HeimatName2", P."HeimatStrasse", P."HeimatAdresszusatz",  
        P."HeimatGemeinde", P."HeimatLand", P."HeimatPLZ", P."HeimatOrt", 
        P."HeimatOrtsteil", P."HeimatAdressgebiet", P."Beruf", P."Staatsangeh1"
      FROM "SchuelerSorgebe" SS
      LEFT JOIN "Schueler" S
      ON  S."Mandant" = SS."Mandant"
      AND S."ID" = SS."Schueler"
      LEFT JOIN "Personen" P
      ON  P."Mandant" = SS."Mandant"
      AND P."ID" = SS."Person"
      WHERE NOT SS."Person" IS NULL 
      UNION 
      SELECT DISTINCT
        SS."Mandant", SS."ID", 
        SS."Familiennr", SS."Verhaeltnis", SS."Sorgerecht", SS."Benachrichtigung", 
        SS."SeriendruckName1", SS."SeriendruckName2", SS."Briefempfaenger", 
        SS."Briefanrede", SS."TelefonPrioritaet", SS."Position", SS."Bemerkung",
        SS."Schueler", S."Vorname", S."Nachname",
        SS."Lehrer", 2, CAST('Lehrer' AS VARCHAR(15)), L."Vorname", L."Nachname", L."Namenszusatz", 
        L."Anrede", L."Strasse", L."Adresszusatz", L."Land", L."PLZ", L."Ort", L."Ortsteil",
        L."Adressgebiet", L."Gemeinde", 
        L."Telefon", L."TelefonDienst", L."Mobil", L."Email",
        L."HeimatName1", L."HeimatName2", L."HeimatStrasse", L."HeimatAdresszusatz",  
        L."HeimatGemeinde", L."HeimatLand", L."HeimatPLZ", L."HeimatOrt", 
        L."HeimatOrtsteil", L."HeimatAdressgebiet", L."Beruf", L."Staatsangeh"
      FROM "SchuelerSorgebe" SS
      LEFT JOIN "Schueler" S
      ON  S."Mandant" = SS."Mandant"
      AND S."ID" = SS."Schueler"
      LEFT JOIN "tblLehrer" L
      ON  L."Mandant" = SS."Mandant"
      AND L."ID" = SS."Lehrer" 
      WHERE NOT SS."Lehrer" IS NULL
      UNION
      SELECT DISTINCT
        SS."Mandant", SS."ID", 
        SS."Familiennr", SS."Verhaeltnis", SS."Sorgerecht", SS."Benachrichtigung", 
        SS."SeriendruckName1", SS."SeriendruckName2", SS."Briefempfaenger", 
        SS."Briefanrede", SS."TelefonPrioritaet", SS."Position", SS."Bemerkung",
        SS."Schueler", S."Vorname", S."Nachname",
        SS."Geschwister", 3, CAST('Geschwister' AS VARCHAR(15)), S2."Vorname", S2."Nachname", 
        S2."Namenszusatz", S2."Anrede", S2."Strasse", S2."Adresszusatz", S2."Land", S2."PLZ", S2."Ort", 
        S2."Ortsteil", S2."Adressgebiet", S2."Gemeinde", 
        S2."Telefon", NULL, S2."Mobil", 
        S2."EMail", S2."HeimatName1", S2."HeimatName2", S2."HeimatStrasse", 
        S2."HeimatAdresszusatz", S2."HeimatGemeinde", S2."HeimatLand", 
        S2."HeimatPLZ", S2."HeimatOrt", S2."HeimatOrtsteil", 
        S2."HeimatAdressgebiet", NULL, S2."Staatsangeh1"
      FROM "SchuelerSorgebe" SS
      LEFT JOIN "Schueler" S
      ON  S."Mandant" = SS."Mandant"
      AND S."ID" = SS."Schueler"
      LEFT JOIN "Schueler" S2
      ON  S2."Mandant" = SS."Mandant"
      AND S2."ID" = SS."Geschwister" 
      WHERE NOT SS."Geschwister" IS NULL
      UNION
      SELECT DISTINCT
        SS."Mandant", SS."ID", 
        SS."Familiennr", SS."Verhaeltnis", SS."Sorgerecht", SS."Benachrichtigung", 
        SS."SeriendruckName1", SS."SeriendruckName2", SS."Briefempfaenger", 
        SS."Briefanrede", SS."TelefonPrioritaet", SS."Position", SS."Bemerkung",
        SS."Schueler", S."Vorname", S."Nachname",
        SS."Sorgebe", 4, CAST('Sorgeberechtigt' AS VARCHAR(15)), SB."Vorname", SB."Nachname", 
        SB."Namenszusatz", SB."Anrede", SB."Strasse", SB."Adresszusatz", SB."Land", SB."PLZ", SB."Ort", 
        SB."Ortsteil", SB."Adressgebiet", SB."Gemeinde",
        SB."TelefonPrivat", SB."TelefonBeruf", SB."Mobil", 
        SB."Email", 
        SB."HeimatName1", SB."HeimatName2", 
        SB."HeimatStrasse", SB."HeimatAdresszusatz", SB."HeimatGemeinde", 
        SB."HeimatLand", SB."HeimatPLZ", SB."HeimatOrt", SB."HeimatOrtsteil", 
        SB."HeimatAdressgebiet", SB."Beruf", SB."Staatsangeh1"         
      FROM "SchuelerSorgebe" SS
      LEFT JOIN "Schueler" S
      ON  S."Mandant" = SS."Mandant"
      AND S."ID" = SS."Schueler"
      LEFT JOIN "Sorgeberechtigte" SB
      ON  SB."Mandant" = SS."Mandant"
      AND SB."ID" = SS."Sorgebe"
      WHERE NOT SS."Sorgebe" IS NULL
    ```

## Columns

This view contains 47 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Mandantenbezogene, eindeutige ID

**`Familiennr`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Verhaeltnis`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Sorgerecht`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Benachrichtigung`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`SeriendruckName1`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`SeriendruckName2`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Briefempfaenger`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Briefanrede`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`TelefonPrioritaet`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Position`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Datensatzpositionierung

**`Bemerkung`**

:   [`BLOB subtype text`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-bnrytypes)

**`Schueler`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`SchuelerVorname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`SchuelerNachname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`TypID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Typ`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`TypBezeichnung`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Vorname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Nachname`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Namenszusatz`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Anrede`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Value | Description
    - | -
    0 | Frau
    1 | Herr
    2 | Frau Dr\.
    3 | Herr Dr\.
    4 | Frau Prof\.
    5 | Herr Prof\.
    6 | Frau Prof\. Dr\.
    7 | Herr Prof\. Dr\.
    : | Ms\.
    ; | Mrs\.
    < | Mr\.

**`Strasse`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Adresszusatz`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Land`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`PLZ`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Ort`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Ortsteil`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Adressgebiet`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Gemeinde`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [Gemeinden](../../tables/gemeinden)

**`TelefonPrivat`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`TelefonBeruf`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Mobil`**

:   [`VARCHAR(30)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Email`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatName1`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatName2`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatStrasse`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatAdresszusatz`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatGemeinde`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatLand`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatPLZ`**

:   [`VARCHAR(10)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatOrt`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatOrtsteil`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`HeimatAdressgebiet`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Beruf`**

:   [`VARCHAR(50)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Staatsangeh`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)
