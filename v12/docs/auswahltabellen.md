# Auswahltabellen

Auswahltabellen dienen einzig und allein dem Zweck kurzfristig für den Druck von Crystal Reports-Berichten mit den Eckdaten des Drucks gefüllt zu werden. Diese Eckdaten entsprechen der Auswahl der Druckdaten in Ihrem Magellan-Modul (Magellan, Magellan-Bibliothek, Magellan-Haushalt & Inventar etc.). Die Daten dienen als Ausgang, um Berichte in Crystal Reports zu erzeugen.

Alle folgenden Tabellen werden über ihre Ansichten angesprochen. Die Benennung der Ansichten ist gleich der Tabellen ohne den Prefix `tbl`.

!!! info ""

    Auswahltabellen und Ansichten haben temporären Charakter. Sie speichern die aktuelle Datensatz-Auswahl in Magellan und dienen als Schnittstelle für die Berichtserstellung in Crystal Reports. Wenn Sie beispielsweise in der Schüler-Gesamtliste mehrere Schüler markieren und dann einen Bericht drucken wollen, so werden die Verweise auf die markierten Schüler in der entsprechenden Auswahl-Ansicht festgehalten. 

Es existieren folgende Auswahl-Ansichten:

Ansicht                                                            | Enthält                                  
------------------------------------------------------------------ | -------
[AuswahlAdressen](..\database\views\auswahladressen)               | Auswahl der Adressen
[AuswahlBetriebe](..\database\views\auswahlbetriebe)               | Auswahl der Betriebe
[AuswahlBewerber](..\database\views\auswahlbewerber)               | Auswahl der Bewerber
[AuswahlBuchungen ](..\database\views\auswahlbuchungen)            | Auswahl der Buchungen
[AuswahlHaushalt](..\database\views\auswahlhaushalt)               | Auswahl der Haushaltsjahre, Haushaltstitel und Haushaltsstellen
[AuswahlInventar](..\database\views\auswahlinventar)               | Auswahl des Inventars
[AuswahlKlassen](..\database\views\auswahlklasen)                  | Auswahl der Klassen
[AuswahlKurslisten](..\database\views\auswahlkurslisten)           | Auswahl der Klassen/Jahrgänge und Fächer/Kurse beim Kurslistendruck
[AuswahlLehrer](..\database\views\auswahllehrer)                   | Auswahl der Lehrer
[AuswahlLieferanten](..\database\views\auswahllieferanten)         | Auswahl der Lieferanten
[AuswahlMandanten](..\database\views\auswahlmandanten)             | Auswahl der Mandanten
[AuswahlMedienAusleihe](..\database\views\auswahlmedienausleihe)   | Auswahl der Medienausleihen
[AuswahlMedienAusleiher](..\database\views\auswahlmedienausleiher) | Auswahl der Medienausleiher
[AuswahlMedienVorgaenge](..\database\views\auswahlmedienvorgaenge) | Auswahl der Medienvorgänge
[AuswahlMedien](..\database\views\auswahlmedien)                   | Auswahl der Medien
[AuswahlPersonen](..\database\views\auswahlpersonen)               | Auswahl der Personen
[AuswahlPruefungslisten](..\database\views\auswahlpruefungslisten) | Auswahl der Prüfungslisten im Abitur
[AuswahlSchueler](..\database\views\auswahlschueler)               | Auswahl der Schüler
[AuswahlSchulen](..\database\views\auswahlschulen)                 | Auswahl der Schulen
[AuswahlSorgebe](..\database\views\auswahlsorgebe)                 | Auswahl der Sorgeberechtigten
[AuswahlSportfeste](..\database\views\auswahlsportfeste)           | Auswahl der Sportfeste
[AuswahlVerlage](..\database\views\auswahlverlage)                 | Auswahl der Verlage
[AuswahlZeugnisse](..\database\views\auswahlzeugnisse)             | Auswahl der Schüler beim Zeugnisdruck

Bei den meisten Auswahl-Ansichten werden neben der eigentlichen Auswahl immer auch der aktuelle Mandant und der aktuelle Zeitraum hinterlegt.
