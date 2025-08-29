## Projekt 4: **Semantic Wikibase**

Mittels [Konzeptbeschreibungen (Concept Description)](https://industrialdigitaltwin.io/aas-specifications/IDTA-01001/v3.2/spec-metamodel/concept-description.html) kann die AAS ein eigenes Wörterbuch definieren, das semantische Definitionen seiner Submodell-Elemente enthält, basierend auf der Data Specification der IEC 61360.
Das [IEC61360-Datentemplate](https://industrialdigitaltwin.io/aas-specifications/IDTA-01003-a/v3.1.1/index.html) ist jedoch nicht für alle Anwendungsfälle gleichermassen gut geeignet.    
<img width="158" height="224" alt="image" src="https://github.com/user-attachments/assets/5928aecf-82ad-48fe-815f-f1e6fa0da4ca" />    

Es gibt eine ergänzende [Guideline](https://industrialdigitaltwin.org/wp-content/uploads/2024/10/2024-10_IDTA_ECLASS_Semantic_Transport_ECLASS_in_AAS_1.0.pdf) zum Mapping von ECLASS-Definitionen.

- Das aktuelle Konzept der AAS Concept Description und semantischen Referenzierungen ist für repositoryübergreifende Anwendungen nur bedingt einsetzbar, vor allem weil es für IRDIs kein hinreichend ausdefiniertes webbasiertes Konzept und keine gemanagte Infrastruktur für repositoryübergreifende CDs gibt. 
- ECLASS und IEC-Referenzinhalte sind nicht hürdenfrei über das Web abfragbar und haben sehr träge Prozesse zur Standardisierung neuer Merkmale
- AAS-Plattformen bringen ein CD-Repository mit, z.B. [Eclipse BaSyx™](https://github.com/eclipse-basyx/basyx-wiki/blob/master/docs/source/content/user_documentation/basyx_components/v2/cd_repository/index.md), CD-Repositories als Teil von AAS-Repositories gelten jedoch nur in dieser lokalen Umgebung. 
- Die jetzigen AAS-Spezifikationen verfolgen keine konsequente Ausrichtung auf eine webbasierte Servicearchitektur, stattdessen dominieren veraltete Konzepte auf IRDI-Basis.

Siehe auch Diskussion unter: https://github.com/admin-shell-io/aas-specs-metamodel/issues/595, https://github.com/admin-shell-io/aas-specs-metamodel/issues/548, https://github.com/admin-shell-io/aas-specs-metamodel/issues/250

[Wikibase](https://de.wikipedia.org/wiki/Wikibase) könnte eine geeignete Plattform sein, um die semantische Referenzierung für die AAS in der Breite zu etablieren. 
URIs kann man frei über Rewrite-Rules auf dem Server definieren: https://www.semantic-mediawiki.org/wiki/Help:Pretty_URIs
Ein Beispiel im Wiki: https://semanticid.aas-connect.com/w/index.php?title=Item:Q21&oldid=207, welches dieses IEC-Merkmal repliziert: https://cdd.iec.ch/cdd/iec61360/iec61360.nsf/PropertiesAllVersions/0112-2---61360_4%23AFD116 
Es iit zu prüfen, ob auch der [SemanticHub von Catena-X](https://userguide.cofinity-x.com/en/articles/312999-semantic-hub) evtl. eine geeignete Plattform sein könnte. 

### Folgende Ziele sollen im Wesentlichen erreicht werden:
- Hin zu auflösbaren URIs und webbasierten Services für semantische Referenzen!
- Niedrigschwelliger Zugang, Schaffung einer offenen Plattform für semantische Ids, bspw. ein Wiki, in dem jeder semantische Definitionen mit auflösenden URIs veröffentlichen kann. 
- Spätere Migration und Weiterleitung auf andere semantische Systeme (wie IEC-CDD, ECLASS, QUDT, etc.) zur hürdenfreien Förderung der Standardisierung ermöglichen.
- Entwicklung einer schlanken Spezifikation hierfür (Registry of Semantics, Prototyping-Plattform, Freigabeprozesse, Community/Governance, …)
- Definition und Bereitstellung von Wikibase-Konfigurationen, die den Workflow optimal unterstützen 


### Folgende Teilaufgaben müssen im Wesentlichen bearbeitet werden:
1. Einarbeitung in die Themen [AAS-Concept Descriptions](https://industrialdigitaltwin.io/aas-specifications/IDTA-01001/v3.2/spec-metamodel/concept-description.html) und [Wikibase](https://de.wikipedia.org/wiki/Wikibase).
3. Dazu auch den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren.
4. Analyse der Problemstellung (https://www.youtube.com/@aas-connect).
2. Ist der SemanticHub von Catena-X evtl. eine geeignete Plattform ? https://userguide.cofinity-x.com/en/articles/312999-semantic-hub
6. Akzeptanzfindung: Die erstellten Lösungen sollen in der Community vorgestellt werden.
7. Test der Applikation gegen eine diverse AAS-Server-Infrastruktur.
