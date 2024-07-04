# Die Struktur

Die Datengrundlage von Magellan 10 ist das relationale Datenbank-Management-System [Firebird](https://firebirdsql.org/) in der Version 4. Firebird ist Open Source und wird durch eine internationale Community aktiv weiterentwickelt.

Der standardmäßige Dateiname der Datenbank lautet `Magellan10.fdb`. Der Zugriff erfolgt durch native Bibliotheken oder aber durch [ODBC](https://learn.microsoft.com/en-us/sql/odbc/microsoft-open-database-connectivity-odbc). Crystal Reports greift über ODBC auf die Magellan-Datenbank zu. Die dafür benötigte Datenquelle wird von Magellan automatisch eingerichtet.

## Tabellen

Tabellen (Englisch: *table*) sind Datenbankobjekte, die sämtliche in einer Datenbank enthaltenen Daten umfassen. Die Daten in einer Tabelle sind logisch in Spalten und Zeilen unterteilt. Jeder Zeile repräsentiert einen Datensatz (z.B. die Stammdaten eines Schülers) und jede Spalte ein Feld im Datensatz (z.B. den Nachnamen des Schülers).

## Ansichten

Ansichten (Englisch *view*) sind virtuelle Tabellen, deren Inhalt durch eine Abfrage definiert werden. Wie bei einer Tabelle besteht auch eine Ansicht aus Zeilen und Spalten. Die Daten stammen aus Tabellen, auf die in der definierenden Abfrage verwiesen wird. 

Oft wiederholte und evtl. komplexere Abfragen können schneller von der Datenbank verarbeitet werden, wenn diese als Ansichten gespeichert sind. Ein weiterer Grund für den Einsatz der Ansichten in Magellan ist die Rechteverwaltung. Ansichten können Teile einer oder mehrerer Tabellen anzeigen und mit Rechten versehen werden. So können Ansichten auf nur einen Teil der Tabellen gelegt werden und diese in entsprechenden Situation, in dem ein Benutzer weniger Daten sehen darf, diese nutzen.

!!! note ""

    Als Beispiel sei hier das Zusammenspiel zwischen der Tabelle `tblLehrer` und der Ansicht `Lehrer` genannt. Die Tabelle `tblLehrer` speichert alle Lehrer in Magellan. Die Ansicht `Lehrer` definiert eine Sichtweise auf die Tabelle `tblLehrer`. Während die Tabelle `tblLehrer` stets alle Lehrer auflistet, sorgt die Ansicht `Lehrer` dafür, dass in den meisten Fällen nur der Lehrer aufgelistet wird, der zum aktuellen Benutzer passt.

Es werden lediglich die Standardtabellen in Magellan durch Ansichten repräsentiert, auf Schlüsseltabellen hingegen wird direkt zugegriffen. Ansichten verhalten sich nach außen hin genauso wie Tabellen, so dass Sie in der Regel nichts weiter beachten müssen.

## Schlüsseltabellen

Alle Tabellen und Ansichten, die den Feldaufbau 

``` csv
Kuerzel, Bezeichnung
```

oder

``` csv
Kuerzel, Schluessel, Bezeichnung
```

besitzen, sind sogenannte Schlüsseltabellen. Sie dienen dazu, die möglichen Werte bestimmter Felder auf eine vorgegebene Liste einzuschränken. Wenn Sie z.B. beim Schüler die Konfession eintragen wollen, so können Sie nur ein Kürzel eintragen, dass in der Schlüsseltabelle „Konfessionen“ definiert ist.

Einige Schlüsseltabellen haben einen etwas anderen Aufbau, sie dienen aber dem gleichen Zweck. Hierzu zählen u.a. die Tabellen `Abschlussjahrgaenge`,  `Abteilungen`, `Banken`, `Berufe`, `Bildungsgaenge`, `Bezirke`, `Bundeslaender`, `Faecher`, `Fachtafeln`, `Gemeinden`, `Kreise`, `Noten`, `Sportfeste`, `Wettkämpfe` und `Verordnungen`.

Schlüsseltabellen machen mehr als 50 Prozent aller Tabellen in Magellan aus.

## Mandanten

Mandanten spielen in Magellan eine zentrale Rolle. Sie ermöglichen die Verwaltung mehrerer organisatorisch eigenständigen Einheiten in einer zentralen Datenbank. So können beispielsweise mehrere Schulen einer Stadt Ihre Daten zentral verwalten. Alle Mandanten sind in der Tabellen `Mandanten` und `MandantenSchulformen` definiert.

## Zeiträume

Zeiträume spielen, ähnlich wie Mandanten, eine zentrale Rolle in Magellan. Sie ermöglichen eine zeitraumbasierte Verwaltung Ihrer Schuldaten. In der Regel handelt es sich bei Zeiträumen um Schulhalbjahre. Durch das Wechseln der Zeiträume können Sie Daten aus dem Blickwinkel unterschiedlicher Halbjahre betrachten. So können Sie die Laufbahnentwicklung einzelner Schüler zurück bis zum Einschulungszeitpunkt betrachten, und das inklusive Fächerzuordnung, Noten und Zeugnisse. Alle Zeiträume sind in der Tabelle Zeitraeume definiert.

## Lehrerdaten

Pro Mandant können beliebig viele Lehrer definiert werden. Die Daten der Lehrer finden Sie in den Tabellen `tblLehrer`, `tblLehrerLehraemter`, `tblLehrerFehlzeiten `und `tblLehrerSollBerechnung`.

## Klassendaten

Pro Mandant können beliebig viele Klassen definiert werden. Jeder Klasse müssen zudem die Zeiträume zugeordnet werden, in denen sie gültig ist. Die Daten der Klassen finden Sie in den Tabellen `Klassen` und `KlassenZeitraeume`.
Bitte beachten Sie, dass eine Klasse in der Rolle eines Oberstufenjahrgangs auftreten kann.

## Schülerdaten

Pro Mandant können beliebig viele Schüler definiert werden.

### Schülerstammdaten

Die Stammdaten der Schüler sind in den Tabellen `Schueler`, `SchuelerSorgebe`, `SchuelerSchulen` und `SchuelerAusbildung` definiert.

### Zeitraumbezogene Schülerdaten

In seiner Laufbahn durchläuft ein Schüler mehrere Klassen und Zeiträume an Ihrer Schule. Diese Angaben werden in den Tabellen `KlassenZeitraeume` `SchuelerKlassen`, `SchuelerZeitraeume`, `SchuelerFachdaten`, `tblSchuelerZeugnisbemerkungen` und `tblSchuelerZeugnisformulare` dokumentiert.

### Schülerdaten fürs Abitur

Daten zum Abitur werden in den Tabellen `SchuelerABI`, `SchuelerABIDetails`, `SchuelerABIZeugnisbemerkungen` und `SchuelerABIZeugnisformulare` abgelegt.

### Berufsbezogene Schülerdaten

Daten zum Berufsschulabschluss werden in den Tabellen `SchuelerBBS`, `SchuelerBBSDetails`, `SchuelerBBSZeugnisbemerkungen` und `SchuelerBBSZeugnisformulare` abgelegt.

### Bundesjugendspiele und Sportfeste

Daten für Bundesjugendspiele und Sportfeste werden in den Tabellen `SchuelerSPF`, `SchuelerSPFDetails` abgelegt.
Bitte beachten Sie, dass ein Bewerber sich syntaktisch nicht von einem Schüler unterscheidet.

## Personendaten

Pro Mandant können beliebig viele Personen definiert werden. Die Daten der Personen finden Sie in der Tabelle `Personen`.

## Sorgeberechtigte

Pro Mandant können beliebig viele Sorgeberechtigte gespeichert werden. Die Daten der Sorgeberechtigten finden Sie in der Tabelle `tblSorgeberechtigte`.

## Betriebe

Pro Mandant können beliebig viele Betriebe gespeichert werden. Die Daten der Betriebe finden Sie in den Tabellen `Betriebe`, `BetriebeBerufe`, `BetriebeBildungsgaenge` und `BetriebeKontakte`.

## Schulen

Schulen werden unabhängig vom Mandanten gespeichert. Die Daten der Schulen finden Sie in den Tabellen `Schulen ` und `SchulenKontakte`.

## Adressen

Pro Mandant können zusätzliche Adressen (z.B. die Adresse des Schulamts) gespeichert werden. Diese Adressen finden Sie in den Tabellen `Adressen` und `AdressenKontakte`

## Medien

Medien bilden die Grundlage der Medienverwaltung. Alle Medien werden in der Tabelle `Medien `gespeichert und sind ebenfalls mandantenfähig. Die Medienverwaltung bildet jedes physische Exemplar zugehörig zum Medium in der Tabelle `MedienExemplare` ab. Detaildaten zu bestimmten Medien finden sich in den Tabellen `Medienarten`, `Medienformate`, `MedienKategorien`, `MedienSchlagworte`, `MedienStichworte` und `MedienZustaende` wieder. Die Verbindung zu Lehrern, Schülern und Personen wird über die Tabelle `MedienAusleiher` definiert. Für die Vorgangsverwaltung stehen `MedienVorgaenge ` und `MedienVormerker` zur Verfügung.

## Inventar

Die Inventarisierung einer Schule wird in der Tabelle `Inventar` abgebildet. Detaildaten zum Inventar finden sich in der Tabelle `InventarExemplare` wieder. Auch das Inventar ist mandantenfähig.

Erwähnenswert ist auch der logische Zusammenhang zwischen Medien und Inventar: Wird die Medienverwaltung eingesetzt, so taucht jedes Medium automatisch auch in der Rolle eines Inventarstücks in Erscheinung.

## Haushalt

Die Verwaltung des Schulhaushalts wird in den Tabellen Haushaltsjahre, `Haushaltstitel`, `Haushaltsstellen` und `Haushaltsmittel` abgebildet. Die registrierten Buchungen finden sich in der Tabelle `Buchungen` wieder.
