# Tabelle **Gemeinden**

## Spalten

Diese Tabelle hat 4 Spalten.

**`Schluessel`**

:   [`VARCHAR(8)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Gemeindeschlüssel

**`EnbreaID`**

:   [`VARCHAR(24)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Externer Identifikator aus ENBREA

**`Name`**

:   [`VARCHAR(40)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Name der Gemeinde

**`Verbandsgemeinde`**

:   [`VARCHAR(3)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Schlüssel der Verbandsgemeinde

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`Gemeinden`**

:   `Schluessel`

## Indizes

Diese Tabelle hat einen Index.

**`PK_GEMEINDEN`**

:   `Schluessel`
