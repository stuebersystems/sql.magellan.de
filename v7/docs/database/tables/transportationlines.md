# Table **TransportationLines**

## Columns

This table contains 8 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [TransportationRoutes](../../tables/transportationroutes)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`InboundRoute`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`OutboundRoute`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [TransportationRoutes](../../tables/transportationroutes)

**`Operator`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Adressen](../../tables/adressen)

**`Code`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

**`Name`**

:   [`VARCHAR(100)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

## Primary key

This table has a primary key.

**`TransportationLines`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_TRANSPORTLINES_OPERATOR`**

:   `Mandant, Operator` » [`Adressen (ID, Mandant)`](../../tables/adressen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_TRANSPORTLINES_OUTROUTES`**

:   `Mandant, OutboundRoute` » [`TransportationRoutes (ID, Mandant)`](../../tables/transportationroutes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indices

This table has 4 indices.

**`FK_TRANSPORTLINES_INROUTES`**

:   `Mandant, InboundRoute`

**`FK_TRANSPORTLINES_OPERATOR`**

:   `Mandant, Operator`

**`FK_TRANSPORTLINES_OUTROUTES`**

:   `Mandant, OutboundRoute`

**`PK_TRANSPORTLINES`**

:   `Mandant, ID`
