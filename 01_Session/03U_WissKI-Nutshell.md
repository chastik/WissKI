
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
* Open source and free virtual research environment for scientific research and cultural heritage data
* Online and via browser usable and combines data modeling + ontology + user interface
* Using an OWL ontology for data structuring e.g. ISO 21127 (CIDOC CRM)
* Integrating authority data like GND – Integrated Authority File (Germany), Getty AAT – Art & Architecture Thesaurus; Other international controlled vocabularies and authority files are Getty ULAN (Union List of Artist Names), Getty TGN (Thesaurus of Geographic Names), Iconclass,...
* FAIR and real Linked Open Data (LOD)
* Based on the Wiki-approach, is modular and flexible while many standards and interfaces are supported 

### Simplified WissKI Architecture

* User Interface  
* Semantic Paths (data model)
* CIDOC CRM (ontology layer)
* RDF Triplestore (data storage)

<img src="../assets/wisski_architektur.png" alt="WissKI Architektur" width="100%">
 
### Core Features

* Semantic data modeling with CIDOC CRM
* Form-based data capture 
* Entity management (actors, objects, places…)
* Pathbuilder
* Modular, easy adjustable and customizable
* SPARQL endpoint, Linked Open Data ready

### Semantic Data Modeling (the WissKI-Way)

<video width="600" controls autoplay loop muted>
  <source src="assets/semantic_modelling.mp4" type="video/mp4">
</video>

▶️ [Video ansehen](../assets/semantic_modelling.mp4)


<video width="600" controls>
  <source src="../assets/semantic_modelling.mp4" type="video/mp4">
  Dein Browser unterstützt das Video-Tag nicht.
</video>


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
| Event        | E5  Event            |
| Place        | E53 Place           |
| Object       | E22 Man-Made Object |
| Time         | E52 Time-Span       |


### Example Knowledge Graph

*A vase was found during an excavation by a research team in Nara in 2005.*

E22 Object → was found by → E5 Event → carried out by → E74 Group
                          
E22 Object → took place at → E53 Place
                          
E22 Object → occurred in → E52 Time-Span




Now that we understand the logic behind WissKI and CIDOC CRM, we will start applying it. In the next unit, we begin modeling our first data entities step by step.













