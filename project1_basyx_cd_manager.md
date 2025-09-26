## Projekt 1: **BaSyx ConceptDescription-Plugin**


["ConceptDescription" (CD)](https://industrialdigitaltwin.io/aas-specifications/IDTA-01001/v3.2/spec-metamodel/concept-description.html) ist ein von der AAS definiertes Konzept für semantische Datenbanken, basierend auf dem [DataSpecificationIec61360-Template](https://industrialdigitaltwin.io/aas-specifications/IDTA-01003-a/v3.1.1/index.html). Für das [BaSyx-GUI-Projekt](https://github.com/eclipse-basyx/basyx-aas-web-ui) gibt es eine Anforderung im Ticket-System für ein [Concept-Description-Plugin](https://github.com/eclipse-basyx/basyx-aas-web-ui/issues/169), was als Grundlage für dieses Projekt verwendet werden soll. 

Das [Open-Source Projekt AAS-Brain](https://github.com/mhrimaz/aasbrain-concept-description-repo) soll auch als Ideenlieferant analysiert werden. 

Das **BaSyx ConceptDescription-Plugin** (aka CD-Manager) soll ein webbasiertes UI bereitstellen, u.A. mit einer sortierbaren Listenansicht ähnlich wie hier:    

<img width="611" height="353" alt="image" src="https://github.com/user-attachments/assets/4a6c7414-e681-4571-97cc-7e36f62b74f9" />

Sowie einem Dialog zum editieren des jeweiligen Datensatz ähnlich wie hier:    
<img width="1820" height="1775" alt="image" src="https://github.com/user-attachments/assets/4e9b2293-7181-4d90-95e2-3ad5a4bd646c" />     

Ergänzend zu den typischen [CRUD-Funktionalitäten](https://de.wikipedia.org/wiki/CRUD) soll ein IEC-Importer implementiert werden, der einen kompletten IEC-CDD-Datensatz in das CD-Repository einlesen kann. 
Hierzu soll die URL auf das entsprechende CDD-Merkmal (z.B. https://cdd.iec.ch/CDD/IEC61360/iec61360.nsf/PropertiesAllVersions/0112-2---61360_4%23AAE530) übergeben werden, dann ein Algorithmus die Inhalte der aufgerufenen Webseite extrahieren und in das Format des [DataSpecificationIec61360-Template](https://industrialdigitaltwin.io/aas-specifications/IDTA-01003-a/v3.1.1/specification.html) überführen.

<img width="634" height="491" alt="image" src="https://github.com/user-attachments/assets/fb6745e0-a731-428a-adef-291e25b0e0a6" />     

**Folgende Teilaufgaben müssen dabei im Wesentlichen bearbeitet werden:**

1. Einarbeitung: Den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und eine [BaySyx-Infrastruktur aufsetzen](https://basyx.org/get-started/introduction).
2. Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken in den Tutorials verbessern.
3. Einarbeitung in das Thema "Concept Descriptions" (z.B. [https://www.youtube.com/@aas-connect](https://www.youtube.com/watch?v=AoRxfgkSVr4)).
4. Forken der benötigten [Basyx-Repositories](https://github.com/eclipse-basyx/basyx-aas-web-ui).
5. Lokale Buildchain einrichten und beherrschen lernen: Änderungen vornehmen, Build-Prozess anstossen, sind die Änderungen sichtbar im lokalen Livesystem?
6. Analyse des [BaSyx-UIs](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html), Definition eines Usability-Konzeptes und Workflows für die CD-Manager-Anwendungsfälle.
7. Implementierung und Test der Funktionalitäten
8. Hosting der Funktionalität auf einem über das Internet zugänglichen Demo-Server
9. Erstellung und Verlinkung einer strukturierten Online-Benutzerdokumentation für das enue Plugin im BaSyx-Github.
10. Akzeptanzfindung für die erstellte Lösung im Open-Source-Projekt herbeiführen

__Beispiel DataSpecificationIec61360-Template in JSON:__
````
{
	"idShort": "Length_CD",
	"displayName": [
		{
			"language": "en",
			"text": "Length"
		},
		{
			"language": "de",
			"text": "Länge"
		}
	],
	"description": [
		{
			"language": "en",
			"text": "for objects with orientation in preferred position during use the dimension perpendicular to diameter/height/width/depth"
		},
		{
			"language": "de",
			"text": "bei eher rechtwinkeligen Körpern die größte orthogonal zu Durchmesser/Höhe/Breite/Tiefe stehende Ausdehnung parallel zu einer Symmetrieachse"
		}
	],
	"administration": {
		"version": "0",
		"revision": "9",
		"creator": {
			"type": "ExternalReference",
			"keys": [
				{
					"type": "GlobalReference",
					"value": "Markus Rentschler (ARENA2036)"
				}
			]
		},
		"templateId": "https://cdd.iec.ch/CDD/IEC61360/iec61360.nsf/PropertiesAllVersions/0112-2---61360_4%23AAF317"
	},
	"id": "0173-1#02-BAA018#007",
	"embeddedDataSpecifications": [
		{
			"dataSpecificationContent": {
				"preferredName": [
					{
						"language": "en",
						"text": "length"
					}
				],
				"unit": "millimetre",
				"unitId": {
					"type": "ExternalReference",
					"referredSemanticId": {
						"type": "ExternalReference",
						"keys": [
							{
								"type": "GlobalReference",
								"value": "https://qudt.org/vocab/unit/MilliM"
							}
						]
					},
					"keys": [
						{
							"type": "GlobalReference",
							"value": "0112/2///62720#UAA862"
						}
					]
				},
				"sourceOfDefinition": "ECLASS",
				"symbol": "mm",
				"dataType": "REAL_MEASURE",
				"levelType": {
					"min": false,
					"nom": true,
					"typ": false,
					"max": false
				},
				"modelType": "DataSpecificationIec61360"
			},
			"dataSpecification": {
				"type": "ExternalReference",
				"keys": [
					{
						"type": "GlobalReference",
						"value": "http://admin-shell.io/DataSpecificationTemplates/DataSpecificationIEC61360/3/0"
					}
				]
			}
		}
	],
	"modelType": "ConceptDescription"
}
````
