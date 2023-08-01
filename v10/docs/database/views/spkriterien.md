# View **SPKriterien**

## Query

??? info "SQL"

    ``` sql
    
      SELECT "Mandant", "SchuelerZeitraumID", 'A' AS "Typ", "TypA", "WertA1", "WertA2", "WertA3"
      FROM "SchuelerPruefungen"  UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'B' AS "Typ", "TypB", "WertB1", "WertB2", "WertB3"
      FROM "SchuelerPruefungen"  UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'C' AS "Typ", "TypC", "WertC1", "WertC2", "WertC3"
      FROM "SchuelerPruefungen"  UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'D' AS "Typ", "TypD", "WertD1", "WertD2", "WertD3"
      FROM "SchuelerPruefungen"  UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'E' AS "Typ", "TypE", "WertE1", "WertE2", "WertE3"
      FROM "SchuelerPruefungen"  UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'F' AS "Typ", "TypF", "WertF1", "WertF2", "WertF3"
      FROM "SchuelerPruefungen"  UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'G' AS "Typ", "TypG", "WertG1", "WertG2", "WertG3"
      FROM "SchuelerPruefungen" 
      UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'H' AS "Typ", "TypH", "WertH1", "WertH2", "WertH3"
      FROM "SchuelerPruefungen"  UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'I' AS "Typ", "TypI", "WertI1", "WertI2", "WertI3"
      FROM "SchuelerPruefungen"  UNION
      SELECT "Mandant", "SchuelerZeitraumID", 'J' AS "Typ", "TypJ", "WertJ1", "WertJ2", "WertJ3"
      FROM "SchuelerPruefungen"
    ```

## Columns

This view contains 7 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Mandanten](../../tables/mandanten)

**`SchuelerZeitraumID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Typ`**

:   [`CHAR(1)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Feld`**

:   [`SMALLINT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Wert1`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Wert2`**

:   [`NUMERIC(?, 4)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-fixedtypes)

**`Wert3`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)
