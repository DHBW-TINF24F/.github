## Projekt 5: **Mnestix Produktkatalog**

Die sog. „Verwaltungsschale“ ([Asset Administration Shell](https://www.plattform-i40.de/IP/Redaktion/DE/Downloads/Publikation/Details_of_the_Asset_Administration_Shell_Part1_V3.html)) ist der Standard der Industrie 4.0 für die Modellierung von digitalen Abbildern (sog. „digitalen Zwillingen“) von Gegenständen wie bspw. Automatisierungsgeräten, -systemen und zu fertigenden Produkten. Von der [IDTA](https://industrialdigitaltwin.org/content-hub/downloads) bereitgestellte Tools wie der AASX Explorer \[3\] dienen zum Erzeugen von dateibasierten Verwaltungsschalen (Typ 1) und sog. reaktive Verwaltungsschalen (Typ 2) können über eine standardisierte REST-API durch sog. AAS Server im Netzwerk bereitgestellt werden. Es existieren Web-Frontends zur Visualisierung, wobei diese eher technisch orientiert und nicht wirklich userfreundlich gestaltet sind.

Im Rahmen der Aufgabe soll das [Produktkatalog-Feature](https://marketplace.arena2036.app/) des Open-Source-Projekt [Mnestix-Browser](https://github.com/eclipse-mnestix/mnestix-browser/tree/1.5.0-product-catalog) weiterentwickelt werden.

<img width="4014" height="2195" alt="image" src="https://github.com/user-attachments/assets/b2cdd752-d044-4dde-8685-ab0266583dca" />

Inhaltlich geht es dabei um einige Fehlerbehebungen, Featureerweiterungen sowie Usability-Verbesserungen:

### Generell:
- Der Login-Status soll ständig sichtbar in der Kopfzeile dargestellt werden.

 ### In der Konfigurationsansicht:
- Im Konfigurationsdialog sollen die Einstelloptionen verfeinert werden: CD-Repositories sollen konfiguriert werden können. Einzelne AAS-Repositories sollen deaktiviert werden können.
- Es soll eine inhaltliche Anzeige des/der CD-Repositories möglich sein.

### In der Katalogauswahl:
- Anzeige der Anzahl der Produkt-Einträge pro Repository.

### In der Produktliste:
- Das Laden der Repositories soll nichtblockierend erfolgen.
- Nur anzeigen von AASen mit AssteKind==Type, Ausblenden von AASen bspw. mit AssetKind == NotApplicable.
- Beim Laden der Shell-Listen sollen per Query-Parametern einstellbare Filterparameter zurückgeliefert werden und somit eine Filterung oder Sortierung der kompletten Shell-Liste ermöglichen.
- Das Laden der Thumbnails/Bilder soll nur für den angezeigten Ausschnitt erfolgen.
- In der Listenansicht Anzeige von Spalten mit ManfacturerName, ProductDesignation, OrderCode, ManufacturerCode und globalAssetId und [createdAt](https://github.com/admin-shell-io/aas-specs-metamodel/issues/484).
- Spaltensortierung soll möglich sein

### In der Produktansicht:
- Der [Nameplate-Generator](https://github.com/TTRSF/TINF22F-Nameplate-Generator) soll in der Produktansicht über das Auswahlmenu integriert werden.
- Die Anzeige des SM BOM soll verlinkte AASen aufrufen können.
- Die Anzeige des SM HandoverDocumentation soll toleranter implementiert und ansprechender formatiert werden (problematische Spaltenformatierungen reduzieren).
- Die Anzeige des SM TechnicalData soll benutzerfreundlicher erfolgen.
- Ergänzung um eShop-Features (addToCart, showCart, etc.)


### Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:

1. Einarbeitung in das Thema AAS und Mnestix. Dazu den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und ein [Mnestix-Frontend](https://github.com/mnestix/mnestix-browser) mit [BaySyx-Infrastruktur](https://basyx.org/get-started/introduction) aufsetzen. Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken verbessern.
2. Analyse der „Concept Description“ (Asset-Reference).
3. Analyse (auch im Vergleich mit anderen AAS-UIs) und Definition eines verbesserten Usability-Konzeptes für die Anzeige von Submodellen im [Mnestix-UI](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html)
4. Forken des [Mnestix-Repositories](https://github.com/mnestix/mnestix-browser), Änderungen vornehmen, Build-Prozess anstossen, Änderungen sichtbar?
5. Umsetzung der Usability-Verbesserungen, Integration der Funktion „Nameplate-Generator“.
6. Akzeptanzfindung: Die erstellten Lösungen sollen in den Mainstream des Mnestix-Projekts eingebracht werden.
7. Test der Applikation gegen eine diverse AAS-Server-Infrastruktur.
