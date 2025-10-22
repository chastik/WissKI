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

Develop and implement your data model 

From collection to diagram - understanding and explaining

Unit 4: CIDOC CRM and Domain Ontologies  - Why CIDOC CRM as underlying ontology?

Duration: approx. 10 Min.

## Why do we use Ontologies?

When we model research data, especially in the cultural heritage and humanities domain, we are not only describing data, but also meaning. Ontologies help us:

* Express semantic relationships
* Make knowledge machine-interpretable
* Ensure interoperability across institutions and systems
* Connect our data with Linked Open Data
* Preserve context and provenance

## Waht is CIDOC CRM?

CIDOC CRM is an ISO standard ontology (ISO 21127) developed by CIDOC, the Documentation Committee of ICOM.
It was designed specifically for cultural heritage, museums, archives, and research documentation.

It focuses on events, actors, objects, places, and time—allowing us to model how things are connected.

* ISO standard ontology for cultural heritage
* Models events, actors, objects, time, and space
* Focuses on context and provenance
* Widely used in DH and GLAM
* * WissKI is based on OWL ontologies and can also use others


## Key Concepts in CIDOC CRM

CIDOC CRM is event-centric:
→ Instead of stating static facts, it models what happened.

| Concept Dimension | Example Class                 | Description                   |
| ----------------- | ----------------------------- | ----------------------------- |
| Thing             | **E70 Thing**                 | Physical or conceptual entity |
| Physical Object   | **E22 Man-Made Object**       | Artefact, specimen, artwork   |
| Actor             | **E21 Person**, **E74 Group** | People or organizations       |
| Event             | **E5 Event**                  | Something that happens        |
| Place             | **E53 Place**                 | Spatial entity                |
| Time              | **E52 Time-Span**             | Temporal extent               |


## Example: Expressing Meaning with CIDOC CRM

*A vase was found during an excavation by a research team in Nara in 2005.*

E22 Object → was found by → E5 Event → carried out by → E74 Group
                          
E22 Object → took place at → E53 Place
                          
E22 Object → occurred in → E52 Time-Span

| Natural Language                    | CIDOC CRM Model                  |
| ----------------------------------- | -------------------------------- |
| The vase is an object               | E22 Man-Made Object              |
| It was found in an excavation       | P12 occurred in → E5 Event       |
| The event was carried out by a team | P14 carried out by → E74 Group   |
| It took place in Nara               | P7 took place at → E53 Place     |
| It happened in 2005                 | P4 has time-span → E52 Time-Span |

So instead of flat metadata, we build context-rich knowledge.

E1 CRM Entity
 └── E5 Event
       └── E7 Activity
 └── E70 Thing
       └── E21 Person
       └── E22 Man-Made Object
 ...

This inheritance structure makes modeling flexible and reusable.

## Domain Ontologies

CIDOC CRM is a core ontology. It can be extended with domain ontologies such as:

CRMsci – Scientific observations

CRMdig – Digitization processes

CRMarchaeo – Archaeological data

FRBRoo / LRMoo – Bibliographic data

MEGA Ontology – Game studies domain (our example today)

These ontologies enrich domain vocabulary while staying compatible with CIDOC CRM.


## Why CIDOC CRM in WissKI?

It is an explicit semantics framework

It supports interoperable cultural heritage data

It integrates well with Pathbuilder modeling

It helps us avoid ambiguous data structures

Ensures future-proof knowledge graphs


Now that we understand how CIDOC CRM structures knowledge, we will start using it.
In the next step, we will analyze a small sample collection together and identify core entities and relationships.


_________________________________________________________________

Erweitern: Top ontologies vs domain ontologies

Ausgehend von E1
Trägerontologie als Mehrwert
alles leitet sich vom top level modell ab
dann CIDOC CRM Struktur - an hand eines Beispiels zeigen

Quelle VErlinken


##  Example Knowledge Graph

Now that we understand the logic behind WissKI and CIDOC CRM, we will start applying it. In the next unit, we begin modeling our first data entities step by step.


