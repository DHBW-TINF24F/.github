## Projekt 2: **BaSyx Viewer-Plugin-Erweiterung**

Für das [BaSyx-GUI-Projekt](https://github.com/eclipse-basyx/basyx-aas-web-ui) gibt es eine Reihe von [Anforderungen im Ticket-System](https://github.com/eclipse-basyx/basyx-applications/issues/240), welche als Anforderungsgrundlage verwendet werden sollen. 

![image](https://github.com/user-attachments/assets/34d6e4bf-d1eb-443f-98cb-9d3f75068bf2)

Für das vorliegende Projekt soll für das BaSyx-UI das AAS-Viewer-Plugin erweitert werden. 
Im Rahmen der Aufgabe soll das Open-Source-Projekt  weiterentwickelt und insbesondere die Usability verbessert werden. Betrachtet werden sollen vor allem die [Submodelle](https://github.com/admin-shell-io/submodel-templates/tree/main/published) 
„**Digital Nameplate**“, „**Technical Data**“, „**HandoverDocumentation**“, „**Hierarchical Structures enabling Bills of Material**“, „**Bill of Process**“, **„ServiceRequestNotification“** sowie **"CommercialData/PurchaseRequest"**. 
Der [Nameplate-Generator](https://github.com/TTRSF/TINF22F-Nameplate-Generator) soll in das [Submodel-Plugin](https://github.com/eclipse-basyx/basyx-aas-web-ui/tree/main/aas-web-ui/src/components/SubmodelPlugins) „Digital Nameplate“ integriert werden. 

__Im Plugin sollen folgende Anwendungsfälle unterstützt werden__:

1. Listensortierung soll möglich sein nach den relevanten Spaltenkriterien. Insbesondere soll die Datumsabhängige Sortierung nach createdAt/updated Atmöglich sein. Hierzu muss ggf. der REST-API-Endpunkt /shells um Query-Parameter erweitert werden.
2. Der Submodell-Baum einer AAS soll angezeigt werden können. Inhaltlich noch nicht vollständig befüllte Submodelle oder Attribute sollen optisch hervorgehoben werden (z.B. rot markiert).


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
