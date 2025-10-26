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

icon: https://github.com/chastik/Beratung_Dateityp_Bild/refs/heads/main/resources/SODa-Logo_full.svg

link: https://raw.githubusercontent.com/chastik/WissKI/refs/heads/main/soda.css

-->

# SODa WissKI-ISWC25 Bits

DEVELOP AND IMPLEMENT YOUR DATA MODEL

From collection to diagram - understanding and explaining

**Unit 4: CIDOC CRM and Domain Ontologies  - Why CIDOC CRM as underlying ontology?**

Duration: ~ 10 Min.

## Why do we use Ontologies?

When we model research data, especially in the cultural heritage and humanities domain, we are not only describing data focusing on contexts and provenance.

Ontologies help us:

* Express semantic relationships
* Make knowledge machine-interpretable
* Ensure interoperability across institutions and systems
* Connect our data with Linked Open Data
* Preserve context and provenance.

## Waht is CIDOC CRM?

![CIDOC CRM](https://cidoc-crm.org/) is an ![ISO standard ontology (ISO 21127)](https://en.wikipedia.org/wiki/International_standard) developed by CIDOC, the International Committee for Documentation of the ![International Concil of Museums (ICOM)](https://icom.museum/en).

It was designed specifically for cultural heritage documentation in galleries, libraries, archives, museums (GLAMs).

It focuses on events, persons, objects, places, time, and spaces as well as their semantic relations. 

**WissKI is based on CIDOC CRM OWL ontology but can also use others!**

## Key Concepts in CIDOC CRM

CIDOC CRM is event-centric:

→ Instead of stating static facts, it models what happened to an object and its context.

| Concept Dimension | Example Class                 | Description                   |
| ----------------- | ----------------------------- | ----------------------------- |
| Thing             | **E70 Thing**                 | Physical or conceptual entity |
| Physical Object   | **E22 Man-Made Object**       | Artefact, specimen, artwork   |
| Actor             | **E21 Person**, **E74 Group** | People or organizations       |
| Event             | **E5 Event**                  | Something that happens        |
| Place             | **E53 Place**                 | Spatial entity                |
| Time              | **E52 Time-Span**             | Temporal extent               |


## Example: Expressing Meaning with CIDOC CRM

*A video game titled "The Legend of Zelda: A Link to the Past" was created by Nintendo in Japan in 1991.*

**Natural Language Assumptions**

The item is a thing.

The (boxed SNES) Zelda game is a physical object.

It was created in a production event.

The production was carried out by Nintendo.

The production took place in Kyoto, Japan.

It happened in 1991.

Its title is “The Legend of Zelda: A Link to the Past”.


**CIDOC CRM Classes**

E22 Object → has title → E35 Title

E22 Object → was created by → E65 Creation → carried out by → E74 Group

E22 Object → was produced at → E53 Place

E22 Object → was created in → E52 Time-Span


…with ZELDA data

E22 Object (SNS Game) → has title → E35 Title (“The Legend of Zelda: A Link to the Past”)

E22 Object → was created by → E65 Creation → carried out by → E74 Group (Nintendo)

E22 Object → was produced at → E53 Place (Kyoto, Japan)

E22 Object → was created in → E52 Time-Span (1991)


### Example: Vase 

*A vase was found during an excavation by a research team in Nara in 2005.*

| Natural Language Description                  | CIDOC CRM Representation                         |
|-----------------------------------------------|--------------------------------------------------|
| The vase is an object                         | E22 Man-Made Object                              |
| It was found in an excavation                 | P12 occurred in → E5 Event                       |
| The excavation was carried out by a team      | P14 carried out by → E74 Group                   |
| The event took place in Nara                  | P7 took place at → E53 Place                     |
| The event happened in 2005                    | P4 has time-span → E52 Time-Span                 |

## From “flat metadata” to knowledge

Instead of flat, record-centric metadata, CIDOC CRM lets us build context-rich knowledge:

E1 CRM Entity
 ├─ E5 Event
 │   └─ E7 Activity
 └─ E70 Thing
     ├─ E21 Person
     └─ E22 Man-Made Object
     
This inheritance structure makes modeling flexible and reusable.

## Top Level Ontologys vs. Domain Ontologys 

In WissKI we use ontologies on two semantic levels:

**Top Level (Core) Ontology**
* Provides a general, shared semantic backbone
* Defines fundamental categories such as Thing, Event, Actor, Place, Time
* Ensures interoperability and consistency across systems
* Example in WissKI: CIDOC CRM as semantic foundation

**Domain Ontologies**
* Extend the core ontology with domain-specific concepts
* Add precision without breaking compatibility
* Used when a field requires richer vocabulary (e.g. archaeology, games, digitization)

Principle:
Use the top ontology to model the general structure of knowledge,
then add domain ontologies to express disciplinary detail.

This two-level approach gives us:
* Semantic clarity
* Interoperability
* Extensibility
* Long-term sustainability of knowledge graphs

## Why CIDOC CRM in WissKI?

* Provides explicit semantics (no ambiguous fields)
* Enables interoperable cultural heritage data
* Integrates well with WissKI Pathbuilder modeling
* Encourages event-centric modeling (context & provenance)
* Supports future-proof knowledge graphs aligned to standards
