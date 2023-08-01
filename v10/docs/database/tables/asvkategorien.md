# Tabelle **ASVKategorien**

## Spalten

Diese Tabelle hat 8 Spalten.

**`Kuerzel`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes) · `NOT NULL`

    Eindeutiges Kürzel

**`Schluessel`**

:   [`VARCHAR(15)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Statistikschlüssel

**`Bezeichnung`**

:   [`VARCHAR(300)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Bezeichnung

**`Art`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [ASVArten](../../tables/asvarten)

**`Gruppe`**

:   [`VARCHAR(20)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

    Verweis auf Tabelle [ASVKategoriegruppen](../../tables/asvkategoriegruppen)

**`StatistikID`**

:   [`VARCHAR(16)`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-chartypes)

**`GueltigVon`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig ab

**`GueltigBis`**

:   [`DATE`](https://firebirdsql.org/file/documentation/html/en/refdocs/fblangref40/firebird-40-language-reference.html#fblangref40-datatypes-datetime)

    Datensatz ist gültig bis

## Primärschlüssel

Diese Tabelle hat einen Primärschlüssel.

**`ASVKategorien`**

:   `Kuerzel`

## Fremdschlüssel

Diese Tabelle hat 2 Fremdschlüssel.

**`FK_ASVKATEGORIEN_GRUPPE`**

:   `Gruppe` » [`ASVKategoriegruppen (Kuerzel)`](../../tables/asvkategoriegruppen) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

**`FK_ASVKATEGORIEN_ART`**

:   `Art` » [`ASVArten (Kuerzel)`](../../tables/asvarten) · `ON UPDATE CASCADE` · `ON DELETE SET NULL`

## Indizes

Diese Tabelle hat 3 Indizes.

**`FK_ASVKATEGORIEN_ART`**

:   `Art`

**`FK_ASVKATEGORIEN_GRUPPE`**

:   `Gruppe`

**`PK_ASVKATEGORIEN`**

:   `Kuerzel`
