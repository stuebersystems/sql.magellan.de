# Table **StoffverteilungenFaecher**

## Columns

This table contains 3 columns.

**`Mandant`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Stoffverteilungen](../../tables/stoffverteilungen)

**`Stoffverteilung`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Stoffverteilungen](../../tables/stoffverteilungen)

**`Fach`**

:   [`INTEGER`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-inttypes) · `NOT NULL`

    Verweis auf Tabelle [Faecher](../../tables/faecher)

## Primary key

This table has a primary key.

**`StoffverteilungenFaecher`**

:   `Mandant, Stoffverteilung, Fach`

## Foreign keys

This table has one foreign key.

**`FK_STOFFFACH_STOFF`**

:   `Mandant, Stoffverteilung` » [`Stoffverteilungen (ID, Mandant)`](../../tables/stoffverteilungen) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

**`FK_STOFFFACH_FACH`**

:   `Fach, Mandant` » [`Faecher (ID, Mandant)`](../../tables/faecher) · `ON UPDATE RESTRICT` · `ON DELETE CASCADE`

## Indices

This table has 3 indices.

**`FK_STOFFFACH_FACH`**

:   `Mandant, Fach`

**`FK_STOFFFACH_STOFF`**

:   `Mandant, Stoffverteilung`

**`PK_STOFFFAECHER`**

:   `Mandant, Stoffverteilung, Fach`
