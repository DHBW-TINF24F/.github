# **Informationen zur Softwaretechnik-Vorlesung TINF24F**

<img src="https://github.com/user-attachments/assets/f499bccf-4b02-42ff-a442-4e11143b32de" alt="Phasen mit Artefekaten" width="650"/>

## **Projektarbeit**

Das vorlesungsbegleitende Software-Projekt soll Ihnen erste Erfahrungen hinsichtlich des Entwurfs, der Implementierung und der Qualitätssicherung von Software in größerem Umfang und innerhalb eines Projektteams geben.

Dies umfasst die typischen Phasen Analyse, Design, Implementierung bis zum Test im abgebildeten Top-Down-Entwicklungsprozess nach einem Phasenmodell.

Es sollen die in den Vorlesungen besprochenen Techniken zur Anwendung kommen.

Es werden Projektthemen mit ähnlichem Schwierigkeitsgrad für 6 Teams angeboten. Bei Unstimmigkeiten unter den Teams, wer welches Projekt machen möchte, treffen die Dozenten die finale Zuweisung. Folgende Themen werden bearbeitet:

### Team 1:  [BaSyx ConceptDescription Manager](https://github.com/DHBW-TINF24F/.github/blob/main/project1_basyx_cd_manager.md)

### Team 2:  [BaSyx Viewer](https://github.com/DHBW-TINF24F/.github/blob/main/project2_basyx_viewer_extension.md)

### Team 3:  [BaSyx Editor](https://github.com/DHBW-TINF24F/.github/blob/main/project3_basyx_editor_extension.md)

### Team 4:  [Semantic Wikibase](https://github.com/DHBW-TINF24F/.github/blob/main/project4_semantic_wikibase.md)

### Team 5:  [Mnestix ProductCatalogue](https://github.com/DHBW-TINF24F/.github/blob/main/project5_mnestix_product_catalogue.md)

### Team 6:  [DPP API](https://github.com/DHBW-TINF24F/.github/blob/main/project6_dpp_api.md)

Jedes Projektteam verwaltet sein Projekt in einem eigenen GIT-Repository mit folgendem Namensschema:   
<https://github.com/DHBW-TINF24F/Team1-Basyx-CD-Manager>

### **FAQ**

**F: Woher kommen die Projektvorschläge?**

A: Die Projektvorschläge wurden von den Dozenten erstellt und sind meist in deren fachlicher Anwendungsdomäne angesiedelt. Das ermöglicht zusätzlichen Wissenstransfer im Rahmen der Projektarbeit. 
Infos zur Einarbeitung: [Tutorials & Resources](https://github.com/DHBW-TINF24F/.github/blob/main/Tutorials.md)

**F: Muss ich alle auch optionalen Features implementieren?**

A: Es besteht kein Zwang, alle optionalen Requirements zu implementieren, wenn die Aufwände zu groß werden. Die optionalen Features dienen als Manövriermasse für Projektrisiken in der Umsetzungsphase.

Sie sind angehalten, eine realistische Umfangsabschätzung der Projektaufgabe durchzuführen, die der eigenen Leistungsfähigkeit im zur Verfügung stehenden Zeitrahmen entspricht. **Entstehen muss am Ende ein funktionierendes und qualitativ überzeugendes sog. „Minimum Viable Product“ (MVP).** Features, die anfangs gemeinsam in der SRS als Mandatory vereinbart wurden, dürfen nicht ohne mit dem Auftraggeber (Dozenten) abgestimmte Begründung fehlen.

**F: Was soll dieses Angebot mit dem Open-Source Projekt?**

A: Um die Wertigkeit der Projektarbeit für Sie zu steigern, wird angeregt, diese im Rahmen von Open-Source-Projekten abzuhandeln. Das hat folgende Vorteile:

- Die Studenten können später in Ihrem Lebenslauf auf Mitarbeit an einem veröffentlichten Open-Source-Projekt verweisen.
- Die Dozenten können die Software von nachfolgenden Studenten-Jahrgängen weiterentwickeln lassen (siehe rechtliche Hinweise weiter unten).

**Beispiele:**

- <https://autarchprinceps.github.io/MultiCastor/>
- <https://github.com/GoranErdeljan/TINF19C-Team-4-Service-Registry>
- <https://github.com/robinziegler/TINF21C_Team4_Modelling_Wizard_Improvements>
- <https://github.com/mercal03/TINF21C_Team1_AAS-Server-Webclient>
- <https://github.com/ilire0/TINF22F_Team-1_AAS-Webclient>
- <https://github.com/MidFidelity/TINF21C_Team2_AAS_digital_nameplate>
- <https://github.com/TTRSF/TINF22F-Team2-Nameplate-Generator>
- <https://github.com/DHBW-TINF23F/Team3-BaSyx-Editor-Plugin>

---

**Rechtliche Hinweise**

- Die erstellte Software ist ihr geistiges Eigentum. Sie haben das Vollkommene und alleinige Nutzungsrecht.
- Die Dozenten werden den Source-Code nicht ohne ihr Einverständnis weiterverwenden.
- Bei Veröffentlichung bzw. Offenlegung (z.B. als Open-Source-Projekt im GitHub-Repository) sind sie selbst für die Formulierung entsprechender Lizenzrechte verantwortlich. Es wird die Verwendung der MIT-Lizenz empfohlen.


## **Verfahrensanweisungen**

## **Rahmenbedingungen**

- Gruppen zu 5-7 Studenten.
- Jeder im Team hat eine oder mehrere bestimmte Rollen und die zugehörigen Aufgaben. Folgende Rollen müssen pro Team besetzt werden:
  - Projektleiter
  - Produktmanager
  - Systemarchitekt (Leitender Entwickler)
  - Testmanager
  - Technischer Redakteur
  - Jeder ist auch Entwickler
- Jeder im Team muss für mindestens ein Programmmodul oder Dokument die Verantwortung inkl. Implementierung übernehmen und dies deutlich kennzeichnen, da es als Grundlage für die individuelle Benotung herangezogen wird.
- Die Projektdokumentation soll in einem GitHub-Repository abgewickelt werden.
- Die Teamsitzungen mit Beschlüssen, Status und Ergebnissen müssen in einem einfach lesbaren Protokoll im Repository (z.B. fortlaufend aktualisiertes Issue im Issue-Tracker) dokumentiert werden.

---

## **Aufgabe im 3. Semester:**

**Analysephase VL-Wochen 1-6**

1. Bilden Sie Gruppen zu 5-7 Studenten und verteilen Sie Rollen wie beschrieben. Diese Gruppen bleiben für das Semester 3 und 4 bestehen.
2. Suchen Sie sich eines der ausgegebenen Projekte aus.
3. Systematisieren Sie die Anforderungen und ergänzen Sie ggf. zusätzliche Kundenanforderungen, die sich im Gespräch mit dem Auftraggeber (Dozenten) ergeben, in einem CRS.
4. Erstellen Sie einen einfachen (!) Business Case (BC), indem Sie von einer fiktiven kommerziellen Auftragsentwicklung ausgehen.
5. Erstellen Sie eine erste Projektplanung für Ihr Team. Verplanen sie maximal 180 Stunden pro Teammitglied (inklusive Administration und Dokumente schreiben).

Achten Sie auf die in der Vorlesung behandelten Themen Requirements Engineering und Systemanalyse. Versuchen Sie, in Ihrer Gruppe durch Reviews zu gut spezifizierten Anforderungen unter Anwendung der geeigneten Modellierungstechniken zu kommen.

**Designphase VL-Wochen 7-11**

1. Legen Sie pro Team ein GitHub-Repository mit dem Root “**TINF24F/TeamNr/ProjektName**” an, in dem Sie ab dann Ihre Projektartefakte verwalten. Legen Sie dazu jeweils eine Verzeichnisstruktur an wie in Kapitel 1.6 „Dokumentation“ beschrieben.
2. Richten Sie im Repository den Issue-Tracker für die diversen Dokumentreviews und das Team-Protokoll ein, mit jeweils einem eigenen Issue pro Dokument (d.h. CRS, BC, SRS, SAS, STP und für jedes MOD). In diesen Issues werden ggf. auch die jeweiligen Dokumentenstände angehängt.
3. Erstellen Sie im Wiki des Repositories das Pflichtenheft (SRS), in dem das System aus Black-Box-Sicht definiert und modelliert wird.
4. Erstellen Sie im Wiki des Repositories die Architekturspezifikation (SAS), modellieren Sie dort das System aus White-Box-Sicht. Leiten Sie die zu implementierenden Module daraus ab und weisen Sie diese im Projektplan als Arbeitspakete den Teammitgliedern zu. Legen Sie eine entsprechende Verzeichnisstruktur für die zugehörigen Sourcecodedateien in GitHub an.
5. Updaten Sie die Projektplanung im Repository („Projects“ in GitHub). Versuchen Sie dabei, die Aufgaben zu parallelisieren und beachten Sie Abhängigkeiten zwischen Arbeitspaketen.
6. **Die Dozenten raten dringend dazu, bereits im 3. Semester mit der Implementierung eines Prototyps zu beginnen, um das Projektrisiko im 4. Semester entsprechend zu verringern.**
7. Jedes Team präsentiert die Ergebnisse des 3. Semesters in einer 20minütigen Präsentation mit anschließender 10minütiger Verteidigung (üblicherweise im letzten Vorlesungstermin).

**Abzugeben sind am Ende des 3. Semesters zwei Tage vor dem Präsentationstermin folgende Dokumente in elektronischer Form in Ihrem GitHub-Repository:**

- CRS, BC, SRS, SAS, Projektplan
- Sitzungsprotokolle
- Präsentation

## **Aufgabe bis Ende des 4. Semesters:**

1. Implementieren Sie das System, testen und integrieren Sie Ihre Module und erstellen Sie dazu die Moduldokumentation (MOD) im Repository.
2. Richten Sie im Repository den Issue-Tracker für den Systemtest ein.
3. Erstellen Sie den Systemtestplan (STP) im Repository.
4. Führen Sie den Systemtest durch und dokumentieren Sie die Ergebnisse in einem Systemtestreport (STR).
5. Finalisieren Sie alle abzugebenden Dokumente.
6. Jedes Team präsentiert seine Ergebnisse in einer 20minütigen Präsentation mit anschließender 10minütiger Verteidigung.

**Abzugeben sind eine Woche vor dem Präsentationstermin sämtliche Projektdokumente in elektronischer Form (PDF und Basisformat) in Ihrem GitHub-Repository:**

- CRS, BC, SRS, SAS, Projektplan, MODs, STP, STR, Benutzer Manual, Protokolle, Sourcen, Executable.

**Am Tag vor der Präsentation ist auch die finale Projektpräsentation bereitzustellen.**

## **Dokumentation**

### **Allgemeines**

- Lehnen Sie sich für die Gliederung von CRS uns SRS an die [IEEE-830](https://de.wikipedia.org/wiki/Software_Requirements_Specification)
- Diese Gliederungsvorlage ist sehr allgemein. Es kann also sein, dass Sie nicht zu allen Punkten, die erwähnt sind, etwas zu schreiben haben.
- Als Ablage wird die Verwendung des Projektwiki des Repositories (GitHub) empfohlen oder eine Struktur von Markdown-Dateien direkt im Repository. 
- Erlaubte Sprachen für die Projektdokumention sind Deutsch und Englisch, für die SAS ist Englisch verpflichtend.

### **Ablage der Dokumente**

Bitte verwenden Sie für die Abgaben und im Repository (GitHub) **IMMER** folgendes Ablageschema. Denken Sie an die Versionierung der Dateien. Die Dateinamen sollen wie folgt aufgebaut sein, das "X" steht für die Projekt/Teamnummer:

**TINF24F_X-CRS-0v1**,

**TINF24F_X-MOD-Modulname-0v1**

CRS, BC, SRS, SAS, MODs, STP, STR, Präsentationen und MeetingMinutes (bzw. Links auf deren Position im Wiki) hier ablegen (keine weiteren Unterverzeichnisse):

**TeamX_Projektname\\PROJECT\\**

Sourcecodedateien in den entsprechenden Unterstrukturen hier ablegen:

**TeamX_Projektname\\SOURCE\\MODY_Modulname**

Das entwickelte ausführbare Programm zusammen mit dem MANUAL hier ablegen:

**TeamX_Projektname\\EXECUTABLE\\**

Bei der Übermittlung der Projektdateien in einem ZIP-Archiv müssen die oben geforderten Verzeichnisstrukturen enthalten sein. In jeder Übermittlung müssen auch die vorherigen bereits übermittelten Dateien miteingepackt sein, d.h. es soll immer ein vollständiger Projektordner übermittelt werden. **Das gibt Ihnen auch die Chance, ggf. noch Korrekturen bei den bereits abgegeben Dateien einzubringen. In dem Fall immer die Versionsnummer des Dokuments hochzählen.**

Es sollen am Schluss alle Dokumente aus Semester 3 und 4 enthalten sein (die neuesten Versionen der Dokumente). 

### **Einzelne Dokumente / Items**

| **CRS** |     |
| --- | --- |
| Zweck: | Beschreibt die Kundenwünsche an das Produkt |
| Umfang: | 5 - 10 Seiten |
| Vorlage: | Ja |
| Methoden: | Strukturierte Anforderung (Schablone), Fließtext, Skizzen der Oberfläche, Use Cases, Anwendungsfälle, Geschäftsvorfälle, ... |
| Inhalt: | Siehe Vorlage |

| **BC** |     |
| --- | --- |
| Zweck: | Kurze Betrachtung der wirtschaftlichen Aspekte des Projekts |
| Umfang: | Max. 4 Seiten |
| Vorlage: | Nein |
| Methoden: | Voll- / Teilkostenrechnung, Verfahren zur Risikoanalyse, ... |
| Inhalt: | Kostenrechnung:<ul><li>Fixe Kosten und Kosten für die einzelnen Arbeitspakete/Phasen.</li></ul>Rentabilitätsrechnung:<ul><li>Wie verdiene ich Geld damit?</li></ul>Erste grobe Projektplanung als GANTT-Diagramm<ul><li>Wie kann ich das Projekt abwickeln?</li></ul> |

| **SRS** |     |
| --- | --- |
| Zweck: | Beschreibt den Produktumfang und fixiert das Feature-Set aus Black-Box-Sicht |
| Umfang: | 10 - 15 Seiten |
| Vorlage: | Ja |
| Methoden: | Trackbare strukturierte Anforderungen, klar formuliert (Schablone), Skizzen der Oberfläche, Prototypen, Use Cases mit Ablaufdiagrammen, ... |
| Inhalt: | Siehe Vorlage |

| **SAS** |     |
| --- | --- |
| Zweck: | Beschreibt die konzeptionelle Lösung des Gesamtsystems (Grey-Box, White-Box) |
| Umfang: | 5 - 15 Seiten |
| Vorlage: | Ja |
| Methoden: | Architektur-, Komponenten-, Klassen-, Kommunikations-, Ablauf- und Sequenzdiagramme, ERM, Datenmodelle, ... |
| Inhalt: | Siehe Vorlage |

| **STP** |     |
| --- | --- |
| Zweck: | Beschreibt die Systemtestfälle und die Testplanung für den Systemtest des Gesamtsystems (Black-Box) |
| Umfang: | 5 - 15 Seiten, ca. 10 ausgearbeitete Testfälle |
| Vorlage: | Ja |
| Methoden: | Anforderungsbasiertes Testen, Äquivalenzklassenbildung, Grenzwertanalyse, Exploratives Testen, Trennung von Testanweisungen und Testdaten |
| Inhalt: | Siehe Vorlage |

| **MeetingMinutes** |     |
| --- | --- |
| Zweck: | Dokumentiert Ihre Projektaktivitäten |
| Umfang: | 10 - 15 Zeilen Status pro Sitzung<br><br>1 Sitzung pro Woche |
| Vorlage: | Nein |
| Methoden: | Fortlaufend ergänztes Dokument mit Inhaltsverzeichnis, für jede Sitzung ein Unterkapitel |
| Inhalt: | Status der Arbeiten, Probleme, Beschlüsse |
| Hinweis: | Fortlaufende Protokolle als Kapitel in einer einzelnen Datei |

| **PM Dokument** |     |
| --- | --- |
| Zweck: | Projektplanung |
| Umfang: | Max. 5 Seiten |
| Vorlage: | Nein, empfohlen wird „Projects“ im GitHub |
| Methoden: | Siehe PM VL |
| Inhalt: | GANTT, PSP |

## **Präsentationen**

**Allgemeines**

- Zeitvorgabe (möglichst genau) 20 min
- Etwa 10 min Fragen
- Sie dürfen selbst entscheiden, wer und wie viele präsentieren.
- Da Sie sehr viele Informationen in 20 Minuten darstellen müssen, überlegen Sie sich genau, was Sie sagen wollen und welche Informationen auf die Folien kommen. Planen Sie daher zur Vorbereitung der Präsentation ausreichend Zeit ein (30 min bis 1h pro Folie!).
- Faustregel für die Anzahl der Folien ist eine nichtanimierte Folie pro Minute, mit Animationen werden es entsprechend weniger Folien.

**Präsentation 1 - BC/CRS/SRS/SAS (3. Semester)**

Inhalt :

- **Teamvorstellung in der PPT mit Namen, Bild, eMail-Adresse, Matrikelnummer und Projektrolle auf der ersten Folie**. Die Dozenten benötigen das um Sie auseinanderhalten und ggf. kontaktieren zu können.
- Vorstellung des Projektes (Master Usecase)
- Darstellung des Funktionsumfangs, Beschreibung der funktionalen und nichtfunktionalen Anforderungen sowie Entscheidung darüber, ob Mandatory oder Optional.
- Business Case (1 Folie)
- Erläutern Sie Ihre Vorgehensweise und verwendete Tools.
- Zeigen Sie, wie Sie modularisiert haben und wie der daraus abgeleitete Projektplan aussieht.
- Beschreiben Sie die Systemarchitektur und die Modularisierung (Top Down)
- Zeigen Sie wesentliche Lösungsansätze aus der SAS (zum Beispiel Paketformat, Anbindung an Java, ERD, ...).
- Bei Bedarf können Sie auch schon Prototypen vorstellen.

**Präsentation 2 - STP/STR/Produkt Präsentation/Selbstkritik (4. Semester)**

Beispielhafter Inhalt:

- Teamvorstellung in der PPT mit Namen, Bild, eMail-Adresse, Matrikelnummer und Projektrolle (erste Folie)
- Vorstellung des Projektes (Master Usecase)
- Produktübersicht (Black-Box)
- Architekturübersicht und Module (White-Box)
- Vorgehensweise beim Testen
- Live Demo
- Fazit / Ausblick

# **Bewertung**

Die Note ergibt sich aus Folgender prozentualer Verteilung der Bewertung der Gruppenarbeit:

- 2/3 kollektive Leistung für die Implementierung, Entwicklungsdokumentation und Präsentation
- 1/3 individuelle Leistung des Einzelnen in seiner Rolle und für sein verantwortliches Modul bzw. Dokument. Bitte sorgen Sie dafür, dass Ihr individueller Beitrag klar identifizierbar ist, auch in den Wiki-Beiträgen im Repository!

