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

## What is CIDOC CRM?

[CIDOC CRM](https://cidoc-crm.org/) is an [ISO standard ontology (ISO 21127)](https://en.wikipedia.org/wiki/International_standard) developed by CIDOC, the International Committee for Documentation of the [International Concil of Museums (ICOM)](https://icom.museum/en).

It was designed specifically for cultural heritage documentation in GLAMs.

It focuses on events, persons, objects, places, time, and spaces as well as their semantic relations. 

**WissKI is based on CIDOC CRM OWL ontology but can also use others!**

## Key Concepts in CIDOC CRM

CIDOC CRM is event-centric:

Instead of stating static facts, it models what happened to an object and its context.

| Concept Dimension | Example Class                 | Description                   |
| ----------------- | ----------------------------- | ----------------------------- |
| Thing             | **E70 Thing**                 | Physical or conceptual entity |
| Physical Object   | **E22 Man-Made Object**       | Artefact, specimen, artwork   |
| Actor             | **E21 Person**, **E74 Group** | People or organizations       |
| Event             | **E5 Event**                  | Something that happens        |
| Place             | **E53 Place**                 | Spatial entity                |
| Time              | **E52 Time-Span**             | Temporal extent               |


## Expressing Meaning with CIDOC CRM

**Example**

*A video game titled "The Legend of Zelda: A Link to the Past" was created by Nintendo in Japan in 1991.*

**Natural Language Assumptions**

* The item is a thing.
* The boxed SNES Zelda game is a physical object.
* It was created in a production event.
* The production was carried out by Nintendo.
* The production took place in Kyoto, Japan.
* It happened in 1991.
* Its title is *The Legend of Zelda: A Link to the Past*.

**CIDOC CRM Classes with ZELDA data** 

* E22 Object (SNS Game) → has title → E35 Title (The Legend of Zelda: A Link to the Past)
* E22 Object → was created by → E65 Creation → carried out by → E74 Group (Nintendo)
* E22 Object → was produced at → E53 Place (Kyoto, Japan)
* E22 Object → was created in → E52 Time-Span (1991)

### Example Vase 

*A vase was found during an excavation by a research team in Nara in 2005.*

| Natural Language Description                  | CIDOC CRM Representation                         |
|-----------------------------------------------|--------------------------------------------------|
| The vase is an object                         | E22 Man-Made Object                              |
| It was found in an excavation                 | P12 occurred in → E5 Event                       |
| The excavation was carried out by a team      | P14 carried out by → E74 Group                   |
| The event took place in Nara                  | P7 took place at → E53 Place                     |
| The event happened in 2005                    | P4 has time-span → E52 Time-Span                 |

## Top Level Ontologys vs. Domain Ontologys 

A top level ontology is used to model the general structure of knowledge while a domain ontology expresses disciplinary details and specifications. Instead of flat, record-centric metadata, CIDOC CRM geneates context-rich knowledge.

**Top Level (Core) Ontology**
* Provides a general, shared semantic backbone, e.g. CIDOC CRM
* Defines fundamental categories such as Thing, Event, Actor, Place, Time
* Ensures interoperability and consistency across systems

**Domain Ontologies**
* Extend the core ontology with domain-specific concepts
* Add precision without breaking compatibility
* Used for controlles vocabulary or authority data 

This two-level approach gives us:
* Semantic clarity
* Interoperability
* Extensibility
* Long-term sustainability 

## Why CIDOC CRM in WissKI?

* Eliminates **semantic ambiguity** by providing explicit, machine-interpretable meaning for all data elements  
* Ensures **semantic interoperability** across institutions and disciplines  
* Provides a **formal ontological framework** compatible with WissKI Pathbuilder  
- Enables **event-centric representation** that preserves context and provenance  
- Supports **FAIR principles** (Findable, Accessible, Interoperable, Reusable)  
- Integrates seamlessly with **Linked Open Data** ecosystems  
- Enables **standard-compliant, sustainable knowledge graphs**





