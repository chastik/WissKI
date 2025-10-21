
<!--
*titel:
*author:in/urheber:in: 
orcid: 
email: SODa@sammlungen.io
*lizenz: cc by
lizenzlink: https://creativecommons.org/
*persistenter OER link: 
language: 
version:  v1
beschreibung: 
format: SODa WissKI How-to-Tutorial
modultitel: 
modul: Unit 1
einheitstitel: Welcome and warm-up 
eiheit: Einheit 1
lernziel: 

baustein:
zielgruppe: https://zenodo.org/records/15574575
gestaltungsprinzip: 
keywords: ???
erstellungsdatum: 

technische metadaten:
medientyp: text
dateiformat: .md
dauer: 
größe:
software: Web

icon: https://sammlungen.io/themes/custom/brause_theme/brause_theme/logo.svg

link: https://raw.githubusercontent.com/chastik/WissKI/refs/heads/main/soda.css

-->

# Develop and implement your data model 

From collection to diagram - understanding and explaining

## WissKI in a Nutshell

**Goal of this unit**

* Understand what WissKI is
* Learn how it uses semantic modeling
* See how CIDOC CRM structures knowledge
* Prepare for the hands-on session


### What is WissKI?

* WissKI = Wissenschaftliche Kommunikations-Infrastruktur
* Open source virtual research environment
* Combines data modeling + ontology + user interface
* Based on Drupal (CMS) + RDF triplestore (e.g. Blazegraph, Fuseki)
* Designed for cultural heritage & research data


### Core Features

* Semantic data modeling with CIDOC CRM
* Semantic Paths instead of relational tables
* Form-based data capture (Perspectives)
* Entity management (actors, objects, places…)
* SPARQL endpoint, Linked Open Data ready
* Supports authority data and SKOS vocabularies (GND, Getty AAT etc.)

### Simplified WissKI Architecture

User Interface  →  WissKI Perspectives (forms)
                →  Semantic Paths (data model)
                →  CIDOC CRM (ontology layer)
                →  RDF Triplestore (data storage)

### Why CIDOC CRM?

* ISO standard ontology for cultural heritage
* Models events, actors, objects, time, and space
* Focuses on context and provenance
* Widely used in DH and GLAM

### Key CIDOC CRM Concepts (Basic Vocabulary)

| Concept Type | Example Class       |
| ------------ | ------------------- |
| Person       | E21 Person          |
| Group        | E74 Group           |
| Event        | E5 Event            |
| Place        | E53 Place           |
| Object       | E22 Man-Made Object |
| Time         | E52 Time-Span       |


### Example Knowledge Graph

*A vase was found during an excavation by a research team in Nara in 2005.*

E22 Object → was found by → E5 Event → carried out by → E74 Group
                          → took place at → E53 Place
                          → occurred in → E52 Time-Span



Now that we understand the logic behind WissKI and CIDOC CRM, we will start applying it. In the next unit, we begin modeling our first data entities step by step.