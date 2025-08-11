# Schlüsselverzeichnisse

Schlüsselverzeichnisse sind Tabellen die überwiegend dazu genutzt werden Listen von Stammdaten zu halten, um diese kontextbezogen anzuzeigen und einzugeben und in diesem Kontext in der Datenbank festzuhalten. Während die Schlüsselverzeichnisse selbst nur die Liste dieser Daten halten, werden die Primärfelder (meistens das Feld `Kuerzel`) in der entsprechenden Kontexttabelle mit dem Verweis auf das Schlüsselverzeichnis gespeichert.

Als Beispiel die Tabelle `Staatsangehoerigkeiten`: Deren Kürzel werden kontextbezogen in den Tabellen `Schüler` und `Lehrer` und `Sorgeberechtigte` gespeichert. Bei den Schülern und Lehrern in den entsprechenden Feldern für die Staatsangehörigkeit, bei den Sorgeberechtigten im Feld für das Geburtsland.

Einige dieser Schlüsselverzeichnisse sind speziell für Statistiken wichtig, deshalb halten diese die Felder „Schluessel“.

Es folgt eine Liste der Schlüsselverzeichnisse in Magellan mit einer Gegenüberstellung des Tabellennamens und der korrespondierenden Bezeichnung in der Magellan-Oberfläche:

Datenbanktabelle                                                            | Oberflächenbezeichnung
--------------------------------------------------------------------------- | ----------------------
[ASVArten](..\database\tables\asvarten)                                     | Arten (ASV)
[ASVBewertungen](..\database\tables\asvbewertungen)                         | Bewertungen (ASV)
[ASVInhaltetafelInhalte](..\database\tables\asvinhaltetafelinhalte)         | Inhaltetafel-Inhalte (ASV)
[ASVInhaltetafeln](..\database\tables\asvinhaltetafeln)                     | Inhaltetafeln (ASV)
[ASVKategoriegruppen](..\database\tables\asvkategoriegruppen)               | Kategoriegruppen (ASV)
[ASVKategorien](..\database\tables\asvkategorien)                           | Kategorien (ASV)
[ASVTafelKategorien](..\database\tables\asvtafelkategorien)                 | Tafelkategorien (ASV)
[ASVTafeln](..\database\tables\asvtafeln)                                   | Tafeln (ASV)
[ASVTypen](..\database\tables\asvtypen)                                     | Typen (ASV)
[Abgangsarten](..\database\tables\abgangsarten)                             | Abgangsarten (Schüler)
[Abordnungsarten](..\database\tables\abordnungsarten)                       | Abordnungsarten
[AbschluesseExtern](..\database\tables\abschluesseextern)                   | Abschlüsse (Extern)
[AbschluesseIntern](..\database\tables\abschluesseintern)                   | Abschlüsse (Intern)
[Abschlussarten](..\database\tables\abschlussarten)                         | Abschlussarten
[Abschlussjahrgaenge](..\database\tables\abschlussjahrgaenge)               | Abschlussjahrgänge
[Abteilungen](..\database\tables\abteilungen)                               | Abteilungen
[Adressenkategorien](..\database\tables\adressenkategorien)                 | Kategorien (Adressen)
[Amtsbez](..\database\tables\amtsbez)                                       | Amtsbezeichnungen
[Arbeitsaemter](..\database\tables\arbeitsaemter)                           | Arbeitsämter
[AssessmentEntries](..\database\tables\assessmententries)                   | Bewertungseinträge
[AssessmentGroups](..\database\tables\assessmentgroups)                     | Bewertungsgruppen
[AssessmentProfiles](..\database\tables\assessmentprofiles)                 | Bewertungsprofile
[Aufnahmepruefungen](..\database\tables\aufnahmepruefungen)                 | Aufnahmeprüfungen
[Banken](..\database\tables\banken)                                         | Banken
[Behinderungsarten](..\database\tables\behinderungsarten)                   | Behinderungsarten
[Berufe](..\database\tables\berufe)                                         | Berufe
[Berufsfelder](..\database\tables\berufsfelder)                             | Berufsfelder
[Beschaeftigungsarten](..\database\tables\beschaeftigungsarten)             | Beschäftigungsarten
[Beschaeftigungsverh](..\database\tables\beschaeftigungsverh)               | Beschäftigungsverhältnisse
[Besoldungen](..\database\tables\besoldungen)                               | Besoldungen
[Besonderheiten](..\database\tables\besonderheiten)                         | Besonderheiten
[BetreuungenAusserschulisch](..\database\tables\betreuungenausserschulisch) | Betreuungen (außerschulisch)
[BetreuungenInnerschulisch](..\database\tables\betreuungeninnerschulisch)   | Betreuungen (innererschulisch)
[Betreuungsformen](..\database\tables\betreuungsformen)                     | Betreuungsformen
[Bevollmaechtigungen](..\database\tables\bevollmaechtigungen)               | Bevollmächtigungen
[Bewerbungsempfehlungen](..\database\tables\bewerbungsempfehlungen)         | Bewerbungsempfehlungen
[Bewerbungsziele](..\database\tables\bewerbungsziele)                       | Bewerbungsziele
[Bezirke](..\database\tables\bezirke)                                       | Bezirke
[Bildungsgaenge](..\database\tables\bildungsgaenge)                         | Bildungsgänge
[Branchen](..\database\tables\branchen)                                     | Branchen
[Buchungsbereiche](..\database\tables\buchungsbereiche)                     | Buchungsbereiche
[Bundeslaender](..\database\tables\bundeslaender)                           | Bundesländer
[Dienstbez](..\database\tables\dienstbez)                                   | Dienstbezeichnungen
[Dienstherren](..\database\tables\dienstherren)                             | Dienstherren
[Dienstverh](..\database\tables\dienstverh)                                 | Dienstverhältnisse
[Disziplinen](..\database\tables\disziplinen)                               | Disziplinen
[Einschulmerkmale](..\database\tables\einschulmerkmale)                     | Einschulmerkmale
[Empfehlungen](..\database\tables\empfehlungen)                             | Empfehlungen
[Entscheidungen](..\database\tables\entscheidungen)                         | Entscheidungen
[Erscheinungsweisen](..\database\tables\erscheinungsweisen)                 | Erscheinungsweisen
[FachNiveaus](..\database\tables\fachniveaus)                               | Fachniveaus
[Fachgruppen](..\database\tables\fachgruppen)                               | Fachgruppen
[Fachrichtungen](..\database\tables\fachrichtungen)                         | Fachrichtungen
[Fachschwerpunkte](..\database\tables\fachschwerpunkte)                     | Fachschwerpunkte
[Fachstati](..\database\tables\fachstati)                                   | Fachstatus
[FachtafelFaecher](..\database\tables\fachtafelfaecher)                     | Fachtafel - Fächer
[Fachtafeln](..\database\tables\fachtafeln)                                 | Fachtafeln
[FaecherThemen](..\database\tables\faecherthemen)                           | Fächer (Themen)
[FaecherUnterpunkte](..\database\tables\faecherunterpunkte)                 | Fächer (Unterpunkte)
[Faecher](..\database\tables\faecher)                                       | Fächer
[Fahrkarten](..\database\tables\fahrkarten)                                 | Fahrkarten
[FoerderSchwerpunkte](..\database\tables\foerderschwerpunkte)               | Förderschwerpunkte
[Foerderungen](..\database\tables\foerderungen)                             | Förderungen
[FremdsprachenNoten](..\database\tables\fremdsprachennoten)                 | Fremdsprachenoten
[Gemeinden](..\database\tables\gemeinden)                                   | Gemeinden
[GradeEntries](..\database\tables\gradeentries)                             | Notensystemeinträge
[GradeSystems](..\database\tables\gradesystems)                             | Notensysteme
[GradeTypes](..\database\tables\gradetypes)                                 | Notenarten
[Haertefaelle](..\database\tables\haertefaelle)                             | Härtefälle
[Herkunftsarten](..\database\tables\herkunftsarten)                         | Herkunftsarten
[Herkunftsunterlagen](..\database\tables\herkunftsunterlagen)               | Herkunftsunterlagen
[Integrationsmerkmale](..\database\tables\integrationsmerkmale)             | Integrationsmerkmale
[InventarKategorien](..\database\tables\inventarkategorien)                 | Kategorien (Inventar)
[Kammern](..\database\tables\kammern)                                       | Kammern
[KlassenBesonderheiten](..\database\tables\klassenbesonderheiten)           | Besonderheiten für Klassen
[KlassenMerkmale](..\database\tables\klassenmerkmale)                       | Merkmale (Klassen)
[Klassenorganisationen](..\database\tables\klassenorganisationen)           | Klassenorganisationen
[Klassenstufen](..\database\tables\klassenstufen)                           | Klassenstufen
[Konfessionen](..\database\tables\konfessionen)                             | Konfessionen
[Krankenkassen](..\database\tables\krankenkassen)                           | Krankenkassen
[Kreise](..\database\tables\kreise)                                         | Kreise
[Kurssprachen](..\database\tables\kurssprachen)                             | Kurssprachen
[Lehraemter](..\database\tables\lehraemter)                                 | Lehrämter
[LehrerAbgaenge](..\database\tables\lehrerabgaenge)                         | Abgangsarten (Lehrer)
[LehrerAusbildung](..\database\tables\lehrerausbildung)                     | Ausbildung (Lehrer)
[LehrerFehlgruende](..\database\tables\lehrerfehlgruende)                   | Fehlgründe (Lehrer)
[LehrerFunktionen](..\database\tables\lehrerfunktionen)                     | Funktionen (Lehrer)
[LehrerMerkmale](..\database\tables\lehrermerkmale)                         | Merkmale (Lehrer)
[LehrerPruefungsbezuege](..\database\tables\lehrerpruefungsbezuege)         | Prüfungsbezüge (Lehrer)
[LehrerSollSchluessel](..\database\tables\lehrersollschluessel)             | Lehrer-Soll-Schlüssel
[LehrerZugaenge](..\database\tables\lehrerzugaenge)                         | Zugangsarten (Lehrer)
[Lehrerkategorien](..\database\tables\lehrerkategorien)                     | Kategorien (Lehrer)
[Leistungsarten](..\database\tables\leistungsarten)                         | Leistungsarten
[MandantenMerkmale](..\database\tables\mandantenmerkmale)                   | Merkmale (Mandanten)
[Mandantenkategorien](..\database\tables\mandantenkategorien)               | Kategorien (Mandanten)
[MedienKategorien ](..\database\tables\medienkategorien)                    | Kategorie (Medien)
[MedienZustaende](..\database\tables\medienzustaende)                       | Medienzustände
[Medienarten](..\database\tables\medienarten)                               | Medienarten
[Medienformate](..\database\tables\medienformate)                           | Medienformate
[MedizinArten](..\database\tables\medizinarten)                             | Medizinarten
[MedizinKategorien](..\database\tables\medizinkategorien)                   | Kategorien (Medizin)
[Muttersprachen](..\database\tables\muttersprachen)                         | Muttersprachen
[Nachpruefungen](..\database\tables\nachpruefungen)                         | Nachprüfungen
[Nachteilsausgleiche](..\database\tables\nachteilsausgleiche)               | Nachteilsausgleiche
[Noten](..\database\tables\noten)                                           | Noten
[Organisationen](..\database\tables\organisationen)                         | Organisationen
[Personenkategorien](..\database\tables\personenkategorien)                 | Kategorien (Personen)
[Postleitzahlen](..\database\tables\postleitzahlen)                         | Postleitzahlen
[Qualifikationsniveaus](..\database\tables\qualifikationsniveaus)           | Qualifikationsniveaus
[Raeume](..\database\tables\raeume)                                         | Räume
[RegionTypes](..\database\tables\regiontypes)                               | Gebietsarten
[Regions](..\database\tables\regions)                                       | Gebiete
[RelGruende](..\database\tables\relgruende)                                 | Religion (Wahlgründe)
[RelTeilnahmen](..\database\tables\relteilnahmen)                           | Religion (Teilnahmen)
[RelWuensche](..\database\tables\relwuensche)                               | Religion (Wünsche)
[Schlagworte](..\database\tables\schlagworte)                               | Schlagworte
[SchuelerArten](..\database\tables\schuelerarten)                           | Schülerarten
[SchuelerBesonderheiten](..\database\tables\schuelerbesonderheiten)         | Besonderheiten für Schüler
[SchuelerFehlgruende](..\database\tables\schuelerfehlgruende)               | Fehlgründe (Schüler)
[SchuelerFunktionen](..\database\tables\schuelerfunktionen)                 | Funktionen (Schüler)
[SchuelerMerkmale](..\database\tables\schuelermerkmale)                     | Merkmale (Schüler)
[SchuelerProfile](..\database\tables\schuelerprofile)                       | Profile (Schüler)
[SchulartenHerkunft](..\database\tables\schulartenherkunft)                 | Schularten (Herkunft)
[Schularten](..\database\tables\schularten)                                 | Schularten
[SchulenMerkmale](..\database\tables\schulenmerkmale)                       | Merkmale (Schulen)
[SchulformenHerkunft](..\database\tables\schulformenherkunft)               | Schulformen (Herkunft)
[SchulformenUebergang](..\database\tables\schulformenuebergang)             | Schulformen (Übergang)
[Schulformen](..\database\tables\schulformen)                               | Schulformen[
[Schulgeldarten](..\database\tables\schulgeldarten)                         | Schulgeldarten
[Schulstati](..\database\tables\schulstati)                                 | Schulstati
[Schulstellen](..\database\tables\schulstellen)                             | Schulstellen
[Schultraeger](..\database\tables\schultraeger)                             | Schulträger
[Schulzweige](..\database\tables\schulzweige)                               | Schulzweige
[Schwerpunkte](..\database\tables\schwerpunkte)                             | Schwerpunkte
[SopaedFoerderungen](..\database\tables\sopaedfoerderungen)                 | Förderbedarf
[SorgebeFunktionen](..\database\tables\sorgebefunktionen)                   |  Funktionen (Sorgeberechtigte)
[Sponsoren](..\database\tables\sponsoren)                                   | Sponsoren
[Sportfeste](..\database\tables\sportfeste)                                 | Sportfeste
[Sprachen](..\database\tables\sprachen)                                     | Sprachen
[Sprachgruppen](..\database\tables\sprachgruppen)                           | Sprachgruppen
[Sprachreferenzen](..\database\tables\sprachreferenzen)                     | Sprachreferenzen
[Staaten](..\database\tables\staaten)                                       | Staaten
[Staatsangehoerigkeiten](..\database\tables\staatsangehoerigkeiten)         | Staatsangehörigkeiten
[Stadtbezirke](..\database\tables\stadtbezirke)                             | Stadtbezirke
[TransportationLines](..\database\tables\transportationlines)               | Verkehrslinien
[TransportationMethods](..\database\tables\transportationmethods)           | Verkehrsmittel (Transportmethode)
[TransportationRoutes](..\database\tables\transportationroutes)             | Fahrtstrecken
[TransportationStops](..\database\tables\transportationstops)               | Haltestellen
[Uebergangsarten](..\database\tables\uebergangsarten)                       | Übergangsarten
[Umschulungsmerkmale](..\database\tables\umschulungsmerkmale)               | Umschulungsmerkmale
[Unterrichtsarten](..\database\tables\unterrichtsarten)                     | Unterrichtsarten
[Unterrichtsformen](..\database\tables\unterrichtsformen)                   | Unterrichtsformen
[Unterstuetzungen](..\database\tables\unterstuetzungen)                     | Unterstuetzungen
[Verkehrsmittel](..\database\tables\verkehrsmittel)                         | Verkehrsmittel
[Verordnungen](..\database\tables\verordnungen)                             | Verordnungen
[Versetzungsarten](..\database\tables\versetzungsarten)                     | Versetzungsarten
[Versicherungsarten](..\database\tables\versicherungsarten)                 | Versicherungsarten
[Vertragsarten](..\database\tables\vertragsarten)                           | Vertragsarten
[Waehrungen](..\database\tables\waehrungen)                                 | Währungen
[Wettkaempfe](..\database\tables\wettkaempfe)                               | Wettkämpfe
[WettkampfDisziplinen](..\database\tables\wettkampfdisziplinen)             | Wettkampf - Disziplinen
[Wiederholungsarten](..\database\tables\wiederholungsarten)                 | Wiederholungsarten
[Wohnformen](..\database\tables\wohnformen)                                 | Wohnformen
[Zeitraeume](..\database\tables\zeitraeume)                                 | Zeiträume
[Zeugnisbemerkungen](..\database\tables\zeugnisbemerkungen)                 | Zeugnisbemerkungen
[Zeugnisbeurteilungen](..\database\tables\zeugnisbeurteilungen)             | Beurteilungen (Zeugnis)
[Zeugnisformulare](..\database\tables\zeugnisformulare)                     | Zeugnisformulare