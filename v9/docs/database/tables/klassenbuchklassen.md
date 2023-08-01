# Tabelle **KlassenbuchKlassen**

## Spalten

Diese Tabelle hat 5 Spalten.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`Klassenbucheintrag`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

**`Klasse`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Klassen](../../tables/klassen)

**`BlockNr`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes)

    Verweis auf Tabelle [Faecher](../../tables/faecher)

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`KlassenbuchKlassen`**

:   `Mandant, Klassenbucheintrag, Klasse`

## Fremdschlüssel

Diese Tabelle hat einen Fremdschlüssel.

**`FK_KBK_KLASSE`**

:   `Klasse, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_KBK_EINTRAG`**

:   `Mandant, Klassenbucheintrag`

**`FK_KBK_KLASSE`**

:   `Mandant, Klasse`

**`PK_KLASSENBUCHKLASSEN`**

:   `Mandant, Klassenbucheintrag, Klasse`
