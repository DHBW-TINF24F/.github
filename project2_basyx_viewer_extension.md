## Projekt 2: **BaSyx Viewer-Plugin-Erweiterung**

Für das vorliegende Projekt soll für das BaSyx-UI das AAS-Viewer-Plugin erweitert werden. 
Für das [BaSyx-GUI-Projekt](https://github.com/eclipse-basyx/basyx-aas-web-ui) gibt es eine Reihe von [Anforderungen im Ticket-System](https://github.com/eclipse-basyx/basyx-aas-web-ui/issues), welche auch als Anforderungsgrundlage verwendet werden sollen. 

![image](https://github.com/user-attachments/assets/34d6e4bf-d1eb-443f-98cb-9d3f75068bf2)

Im Rahmen der Aufgabe soll das Open-Source-Projekt  weiterentwickelt und insbesondere die Usability verbessert werden. Betrachtet werden sollen vor allem die [Submodelle](https://github.com/admin-shell-io/submodel-templates/tree/main/published) 
„**Digital Nameplate**“, „**Technical Data**“, „**HandoverDocumentation**“, „**Hierarchical Structures enabling Bills of Material**“, „**Bill of Process**“, **„ServiceRequestNotification“** sowie **"CommercialData/PurchaseRequest"**. 
Der [Nameplate-Generator](https://github.com/TTRSF/TINF22F-Nameplate-Generator) soll in das [Submodel-Plugin](https://github.com/eclipse-basyx/basyx-aas-web-ui/tree/main/aas-web-ui/src/components/SubmodelPlugins) „Digital Nameplate“ integriert werden. 

- Die AAS-Übesicht soll Listensortierung/-filteung nach relevanten Spaltenkriterien untestützen (z.B. ManfacturerName, ProductDesignation, OrderCode, ManufacturerCode und globalAssetId und createdAt).
- Insbesondere soll die datumsabhängige Sortierung nach createdAt/updatedAt möglich sein. Hierzu muss ggf. der REST-API-Endpunkt /shells um Query-Parameter erweitert werden.
- Beim Laden der Shell-Listen sollen damit per Query-Parametern einstellbare Filterparameter zurückgeliefert werden und somit eine Filterung oder Sortierung der kompletten Shell-Liste ermöglichen.
- Das Laden der Thumbnails/Bilder soll nur für den angezeigten Ausschnitt erfolgen.

**Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:**

1. Einarbeitung: Den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction). Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken in den Tutorials verbessern.
2. Forken der benötigten [Basyx-Repositories](https://github.com/eclipse-basyx/basyx-aas-web-ui).
3. Lokale Buildchain einrichten und beherrschen lernen: Änderungen vornehmen, Build-Prozess anstossen, sind die Änderungen sichtbar im lokalen Livesystem?
4. Analyse des [BaSyx-UIs](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html), insbesondere der DPP-Lösung von HARTING. Das Projekt [AAS-Manager](https://github.com/rwth-iat/aas_manager) ist ebenfalls in Betracht zu ziehen.
5. Definition eines Usability-Konzeptes und Workflows für die Viewer-Anwendungsfälle.
6. Implementierung und Test der Funktionalitäten
7. Hosting der Funktionalität auf einem über das Internet zugänglichen Demo-Server
8. Erstellung und Verlinkung einer strukturierten Online-Benutzerdokumentation im BaSyx-Github.
9. Akzeptanzfindung für die erstellte Lösung im Open-Source-Projekt herbeiführen
