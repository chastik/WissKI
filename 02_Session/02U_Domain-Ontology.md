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
einheitstitel: 
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

icon: /assets/SODa-Logo_full.svg

link: https://raw.githubusercontent.com/chastik/WissKI/refs/heads/main/soda.css

-->

# Develop and implement your data model 

From diagram to paths - applying and xxxx evaluating?

### Domain Ontology Modelling with Draw.io

From conceptual structure to semantic paths (20 min – Interactive Pair Work)

### Why we start with draw.io?

Before implementing anything in WissKI, we first need a clear semantic structure of our data model.
draw.io is a lightweight ontology modeling tool for visually designing entities and relationships.
It allows us to:

* Define entity classes
* Show semantic relationships
* Prepare clean ontology logic
* Collaboratively model before implementation

This step prevents inconsistent modeling later in WissKI and helps us think semantically before building technically.

### What we are modeling

We will model part of the Game Collection domain as an example.
You will work in pairs and model a small domain subgraph based on your interests.

| Option | Scope                                             |
| ------ | ------------------------------------------------- |
| A      | Game → released on → Platform                     |
| B      | Game → created by → Developer/Contributor         |
| C      | Game → has genre, edition, version                |
| D      | Game → has story description → narrative elements |
| E      | Game copy → has inventory → stored at location    |

### Modeling Rules

**Entities should be classes, not data**
✔ Game (Class)   
✔ Platform (Class)   
✔ Release Event (Class)  
✘ “Nintendo Switch” (no – this is an instance, not a class)

**Relationships should have semantic verbs**

* game → was released in → release event
* game → was developed by → group/person

**Attributes become datatype properties**

* game → has title → string
* release → has year → date

### CIDOC CRM Mapping Reminder

* Use CIDOC CRM classes when possible:
* Use domain-specific subclasses only where necessary (e.g. from MEGA Ontology).

### Task (Pair Work – 15 minutes) Step-by-Step Instructions

Goal: Model a small part of the domain using draw.io
Steps:

1. Choose one of the focus topics (A–E)
2. Identify entities
3. Connect them with semantic relationships
4. Use CIDOC CRM classes as superclasses
5. Keep your model clean and readable
6. Save and export your model

* Model 4–6 entities from your domain
* Connect them with CIDOC-compatible relationships
* Identify 1–2 meaningful core paths
* Keep the structure modular and reusable
* Each pair will later briefly present one path and explain their modeling decisions.


### Output

* Each pair creates:

* A small ontology diagram
* Correct semantic relations
* CIDOC CRM backbone
* Ready for Pipeline export in the next unit

### Support

will walk around and support with:

Mapping questions

CIDOC CRM decisions

Modeling strategy

* Place key entities (e.g., Game, Physical Copy, Publisher)
* Connect entities with semantic relationships
* Group related concepts into semantic clusters
* Highlight core paths starting from a central entity
* Set Attributes

### Technical Background – Why Draw.io?

This modeling step is not just a visual exercise — the diagram is part of an (semi)automated pipeline (web-service).....


Once our domain diagrams are ready, we will transform them into WissKI Paths in the next step.



