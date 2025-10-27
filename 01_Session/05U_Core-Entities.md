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

Unit 5: Identify core entities from a collection - Joint exploration

Duration: ~ 20 Min.

### Learning Goal

In this unit, we move from theory to practice. 

In groups, we will:

* analyze a small domain example
* identify core entities and relationships
* understand the difference between domain concepts and semantic classes
* prepare a conceptual model that we will later formalize in Protégé and WissKI.

## Scenario: Extending the MEGA Ontology

In this session, we will extend the MEGA Ontology using a sample collection of computer games. 

The goal is to enrich the semantic model with additional domain concepts relevant for collection management and research.

### Focus of the Extension

- **Game title**
- **Game characteristics**
  - Platform (e.g. Nintendo 64, PlayStation, PC)
  - Genre (e.g. Action-adventure, RPG)
  - Edition or version (e.g. Collector’s Edition, Remastered)
- **Game narrative elements**
  - Perspective (e.g. first-person, third-person)
  - Game description
  - Game Characters

### Why this domain?

This example domain is well suited for semantic modeling because it contains:

- Physical and digital representations of objects
- Creation and production context (developers, publishers)
- Event structures (release events)
- Versions and editions
- Identifiers and collection metadata

### Modeling Goals

- Identify core entities of the domain
- Define meaningful relationships between entities
- Map these entities to suitable CIDOC CRM classes (Version 7.1.3 (February 2024) https://cidoc-crm.org/sites/default/files/cidoc_crm_version_7.1.3.pdf) 
- Develop a shared understanding of the domain structure

### Example Objects from the Collection

| Domain Element    | Example                                |
| ----------------- | -------------------------------------- |
| Game title        | *The Legend of Zelda: Ocarina of Time* |
| Release year      | 1998                                   |
| Publisher         | Nintendo                               |
| Platform          | Nintendo 64                            |
| Creator/Developer | Nintendo EAD                           |
| Contribution      | Composer: Koji Kondo                   |


## Quick CIDOC CRM Demonstration

Before modeling, we briefly explore how the (CIDOC CRM specification (v7.1.3))[https://cidoc-crm.org/sites/default/files/cidoc_crm_version_7.1.3.pdf] defines basic classes.

This helps us recognize entity types and choose appropriate semantic mappings.

Examples from the CIDOC CRM class hierarchy:

| CIDOC CRM Class             | Meaning                                       |
| --------------------------- | --------------------------------------------- |
| **E28 Conceptual Object**   | Game as intellectual content                  |
| **E84 Information Carrier** | Physical copy of the game                     |
| **E21 Person**              | Composer, designer, individual contributor    |
| **E74 Group**               | Development studio, publisher                 |
| **E12 Production**          | Release event or game publication             |
| **E42 Identifier**          | Product code, inventory number, serial number |


## Group Task

You will work in small groups (3–4 people).

Your task: create a semantic mindmap of the domain focussing on game characteristics (platform, genre, edition/version) and narrative elements (perspective, description, character).

Each group will write down ideas using pen and paper or sticky notes.

### Group Work Brainstorming

| Step | Question                              | Goal                            |
| ---- | ------------------------------------- | ------------------------------- |
| 1    | What are the core entities?           | Identify domain building blocks |
| 2    | Which relationships connect them?     | Capture relations               |
| 3    | Which properties or attributes exist? | Add metadata                    |
| 4    | How could these map to CIDOC CRM?     | Anchor in ontology              |
| 5    | Which belong to MEGA Ontology?        | Domain extension awareness      |


### CIDOC CRM Mapping (Examples) - Help Table

| Domain Concept      | CIDOC CRM Suggestion    |
| ------------------- | ----------------------- |
| Game (conceptual)   | E28 Conceptual Object   |
| Physical copy       | E84 Information Carrier |
| Developer/Publisher | E21 Person / E74 Group  |
| Release event       | E12 Production          |
| Identifier          | E42 Identifier          |

### Output of the Group Exercise

Together we will collect and compare the group results.  

Each group can presents briefly:

- 3–5 core entities 
- the relationships between them
- a first CIDOC CRM class mappings


______________________________________

Goal:

Show difference between internal museum metadata (inventory number) and external publication metadata (ISBN/product code)

CIDOC mapping:

Both → E42 Identifier

But different property paths:

Inventory number → identity of physical item (E84 Information Carrier)

ISBN → identity of conceptual work/product (E28 Conceptual Object)


### Open Questions

Let's clarify open modeling questions before moving into Protégé.

(Übergang zu Unit 5, we will formalize your domain concepts as classes and relationships using Protégé.)

- One observation or modeling challenge






