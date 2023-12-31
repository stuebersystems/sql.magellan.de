# Tabelle **StudentRoutes**

## Spalten

Diese Tabelle hat 9 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [TransportationStops](../../tables/transportationstops)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Line`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [TransportationLines](../../tables/transportationlines)

**`Method`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [TransportationMethods](../../tables/transportationmethods)

**`Origin`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [TransportationStops](../../tables/transportationstops)

**`Destination`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`Distance`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

**`Duration`**

:   [`FLOAT`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-floattypes)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`StudentRoutes`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 4 Fremdschlüssel.

**`FK_STUDENTROUTES_LINES`**

:   `Line, Mandant` » [`TransportationLines (ID, Mandant)`](../../tables/transportationlines) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_STUDENTROUTES_METHODS`**

:   `Mandant, Method` » [`TransportationMethods (ID, Mandant)`](../../tables/transportationmethods) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_STUDENTROUTES_ORIGIN`**

:   `Mandant, Origin` » [`TransportationStops (ID, Mandant)`](../../tables/transportationstops) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_STUDENTROUTES_DESTINATION`**

:   `Destination, Mandant` » [`TransportationStops (ID, Mandant)`](../../tables/transportationstops) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 5 Indizes.

**`FK_STUDENTROUTES_DESTINATION`**

:   `Mandant, Destination`

**`FK_STUDENTROUTES_LINES`**

:   `Mandant, Line`

**`FK_STUDENTROUTES_METHODS`**

:   `Mandant, Method`

**`FK_STUDENTROUTES_ORIGIN`**

:   `Mandant, Origin`

**`PK_STUDENTROUTES`**

:   `Mandant, ID`
