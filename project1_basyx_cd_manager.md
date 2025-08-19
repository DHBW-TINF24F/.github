## Projekt 1: **BaSyx ConceptDescription-Plugin**


"ConceptDescription" (CD) ist ein von der AAS definiertes Konzept für semantische Datenbanken, basierend auf dem [DataSpecificationIec61360-Template](https://industrialdigitaltwin.io/aas-specifications/IDTA-01003-a/v3.1.1/index.html). Für das [BaSyx-GUI-Projekt](https://github.com/eclipse-basyx/basyx-aas-web-ui) gibt es eine Anforderung im Ticket-System für einen [Concept-Description-Manager](https://github.com/eclipse-basyx/basyx-aas-web-ui/issues/169), was als Grundlage für dieses Projekt verwendet werden soll. 

Der CD-Manager soll eine sortierbare Listenansicht ähnlich wie hier bereitstellen: 
<img width="1578" height="845" alt="image" src="https://github.com/user-attachments/assets/1b0df5f9-2a12-489e-8af2-a2c4fa53cb87" />

Ergänzend soll ein IEC-Importer implementiert werden, der einen kompletten IEC-CDD-Datensatz in das CD-Repository überführen kann. 
Hierzu soll die URL auf das CDD-Merkmal (z.B. https://cdd.iec.ch/CDD/IEC61360/iec61360.nsf/PropertiesAllVersions/0112-2---61360_4%23AAE530) übergeben werden, dann ein Algorithmus auf dieser Webseite die Inhalte extrahieren und in das [DataSpecificationIec61360-Template](https://industrialdigitaltwin.io/aas-specifications/IDTA-01003-a/v3.1.1/index.html) überführen.

<img width="2347" height="1220" alt="image" src="https://github.com/user-attachments/assets/cb7c3f4c-7fe1-4402-ac27-e008acc1e49f" />


**Folgende Teilaufgaben müssen dabei im Wesentlichen bearbeitet werden:**

1. Einarbeitung: Den [AASX-Explorer](https://github.com/eclipse-aaspe/package-explorer/releases) installieren und eine BaySyx-Infrastruktur [aufsetzen](https://basyx.org/get-started/introduction) aufsetzen.
2. Hierzu die vorhandenen Tutorials anwenden, bewerten und identifizierte Lücken in den Tutorials verbessern.
3. Einarbeitung in das Thema "Concept Descriptions" (z.B. [https://www.youtube.com/@aas-connect](https://www.youtube.com/watch?v=AoRxfgkSVr4)).
4. Forken der benötigten [Basyx-Repositories](https://github.com/eclipse-basyx/basyx-aas-web-ui).
5. Lokale Buildchain einrichten und beherrschen lernen: Änderungen vornehmen, Build-Prozess anstossen, sind die Änderungen sichtbar im lokalen Livesystem?
6. Analyse des [BaSyx-UIs](https://wiki.basyx.org/en/latest/content/user_documentation/basyx_components/web_ui/index.html), Definition eines Usability-Konzeptes und Workflows für die CD-Manager-Anwendungsfälle.
7. Implementierung und Test der Funktionalitäten
8. Hosting der Funktionalität auf einem über das Internet zugänglichen Demo-Server
9. Erstellung und Verlinkung einer strukturierten Online-Benutzerdokumentation im BaSyx-Github.
10. Akzeptanzfindung für die erstellte Lösung im Open-Source-Projekt herbeiführen

__Example DataSpecificationIec61360-Template in JSON:__
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
