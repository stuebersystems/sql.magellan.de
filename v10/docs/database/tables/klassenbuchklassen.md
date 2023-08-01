# Table **KlassenbuchKlassen**

## Columns

This table contains 5 columns.

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

## Primary key

This table has a primary key.

**`KlassenbuchKlassen`**

:   `Mandant, Klassenbucheintrag, Klasse`

## Foreign keys

This table has one foreign key.

**`FK_KBK_KLASSE`**

:   `Klasse, Mandant` » [`Klassen (ID, Mandant)`](../../tables/klassen) · `ON UPDATE RESTRICT` · `ON DELETE RESTRICT`

**`FK_KBK_EINTRAG`**

:   `Klassenbucheintrag, Mandant` » [`Klassenbuch (ID, Mandant)`](../../tables/klassenbuch) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_KBK_EINTRAG`**

:   `Mandant, Klassenbucheintrag`

**`FK_KBK_KLASSE`**

:   `Mandant, Klasse`

**`PK_KLASSENBUCHKLASSEN`**

:   `Mandant, Klassenbucheintrag, Klasse`
