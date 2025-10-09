## Projekt 3: **BaSyx Editor-Plugin-Erweiterung**

Für das [BaSyx-GUI-Projekt](https://github.com/eclipse-basyx/basyx-aas-web-ui) gibt es bereits eine Reihe von [Anforderungen im Ticket-System](https://github.com/eclipse-basyx/basyx-applications/issues/240), welche als Anforderungsgrundlage verwendet werden sollen.
Eine spezifische Anforderung zur Erweiterung der REST-API kann über https://github.com/admin-shell-io/aas-specs-api/issues/286 eingesehen werden. 

Für das vorliegende Projekt soll für das BaSyx-UI das Editor-Plugin, das Viewer-Plugin und das REST-API-Backend erweitert werden: 
![image](https://github.com/user-attachments/assets/34d6e4bf-d1eb-443f-98cb-9d3f75068bf2)    

**Es sollen folgende Anwendungsfälle unterstützt werden:**
1. Externe Modell-Dateien sollen zur AAS hinzugefügt werden können. Nach einer Plausibilitätsprüfung soll eine definitionsgemäße Verlinkung mit passendem MimeType der ausgewählten Datei in der Verwaltungsschale erfolgen.
2. Beim Hinzufügen einer KBL- oder VEC-Datei soll diese inhaltlich analysiert werden können um die Nameplate-Informationen sowie relevante Technischen Daten (z.B. Gewicht, Features des Leitungssatzes) zu extrahieren und in das AAS-Submodel „[General Technical Data](https://github.com/admin-shell-io/submodel-templates/tree/main/published/Technical_Data/1/2)“ zu überführen.
3. Die REST-API soll erweitert werden (siehe https://github.com/admin-shell-io/aas-specs-api/issues/286), um in angehängte XML-Dateien "hineingreifen" zu können.
4. Die internen Datenpunkte einer angehängten XML-Datei sollen strukturiert im Viewer angezeigt werden können. 

**Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:**
1. Eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction). Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken in den Tutorials verbessern.
2. Forken der benötigten [Basyx-Repositories](https://github.com/eclipse-basyx/basyx-aas-web-ui).
3. Lokale Buildchain einrichten und beherrschen lernen: Änderungen vornehmen, Build-Prozess anstossen, sind die Änderungen sichtbar im lokalen Livesystem?
4. Analyse des [BaSyx-UIs](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html), Definition eines Usability-Konzeptes und Workflows für die Editor- und Viewer-Anwendungsfälle.
5. Implementierung und Test der Funktionalitäten
6. Hosting der Funktionalität auf einem über das Internet zugänglichen Demo-Server
7. Erstellung und Verlinkung einer strukturierten Online-Benutzerdokumentation im BaSyx-Github.
8. Akzeptanzfindung für die erstellte Lösung im Open-Source-Projekt herbeiführen
