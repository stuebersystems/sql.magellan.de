# Tabelle **StudentTransportation**

## Spalten

Diese Tabelle hat 6 Spalten.

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

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`StudentTransportation`**

:   `Mandant, ID`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_STUDENTTRANSPORT_OUTROUTES`**

:   `Mandant, OutboundRoute` » [`StudentRoutes (ID, Mandant)`](../../tables/studentroutes) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_STUDENTTRANSPORT_SCHUELER`**

:   `Mandant, Student` » [`Schueler (ID, Mandant)`](../../tables/schueler) · `ON UPDATE CASCADE` · `ON DELETE CASCADE`

## Indizes

Diese Tabelle hat 4 Indizes.

**`FK_STUDENTTRANSPORT_INROUTES`**

:   `Mandant, InboundRoute`

**`FK_STUDENTTRANSPORT_OUTROUTES`**

:   `Mandant, OutboundRoute`

**`FK_STUDENTTRANSPORT_SCHUELER`**

:   `Mandant, Student`

**`PK_STUDENTTRANSPORT`**

:   `Mandant, ID`
