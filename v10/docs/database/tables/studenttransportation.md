# Table **StudentTransportation**

## Columns

This table contains 6 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`ID`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Mandantenbezogene, eindeutige ID

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Student`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Schueler](../../tables/schueler)

**`InboundRoute`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

**`OutboundRoute`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [StudentRoutes](../../tables/studentroutes)

## Primary key

This table has a primary key.

**`StudentTransportation`**

:   `Mandant, ID`

## Foreign keys

This table has one foreign key.

**`FK_STUDENTTRANSPORT_OUTROUTES`**

:   `Mandant, OutboundRoute` » [`StudentRoutes (ID, Mandant)`](../../tables/studentroutes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_STUDENTTRANSPORT_SCHUELER`**

:   `Mandant, Student` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

**`FK_STUDENTTRANSPORT_INROUTES`**

:   `InboundRoute, Mandant` » [`StudentRoutes (ID, Mandant)`](../../tables/studentroutes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indices

This table has 4 indices.

**`FK_STUDENTTRANSPORT_INROUTES`**

:   `Mandant, InboundRoute`

**`FK_STUDENTTRANSPORT_OUTROUTES`**

:   `Mandant, OutboundRoute`

**`FK_STUDENTTRANSPORT_SCHUELER`**

:   `Mandant, Student`

**`PK_STUDENTTRANSPORT`**

:   `Mandant, ID`
