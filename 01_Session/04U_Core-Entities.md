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

# Develop and implement your data model 

From collection to diagram - understanding and explaining

## Joint exploration using the a domain ontology in Protégé


### Learning Goal

* Identify domain core entities and relationships
* Translate inot CIDOC CRM ontology classes
* Map the classes to domain concepts to CIDOC CRM
* Prepare a shared conceptual model for later semantic modeling
* Recognize the role of domain ontologies

### Setup

* Method: Group work (3–4 people per group)
* Material: Sticky notes or small cards + pens OR Etherpad/Miro / Laoptop
* Example domain: Computer game collection (based on MEGA ontology example)

### Your Task

n groups you analyze a small collection scenario and identify the key entities and relationships of the domain. 

This will be the conceptual foundation for our later semantic modeling. 

Each group works collaboratively and prepares a short result presentation.

### The Scenario

A museum holds a collection of computer games. 

Each game has a title, release year, and publisher. 

The museum keeps physical copies of the games, which are stored under inventory numbers. 

Some games have contributors such as designers and composers. 

Each game is published for one or more platforms and may have a digital version available online.


### Group Work Brainstorming

| Step | Question                                                 | Goal                       |
| ---- | -------------------------------------------------------- | -------------------------- |
| 1    | What are we talking about?                               | Define domain and scope    |
| 2    | Which **entities** exist?                                | Identify important objects |
| 3    | Which **relationships** exist?                           | Connect entities           |
| 4    | Which **attributes** or identifiers exist?               | Domain-specific metadata   |
| 5    | How do these map to **CIDOC CRM** classes?               | Semantic grounding         |
| 6    | Which entities belong to the **domain ontology (MEGA)**? | Extend semantic meaning    |


### Support Material

Possible MEGA domain classes:

* Game, GameSeries, Publisher, Platform, Developer, Release, PhysicalCopy
* Identifiers: InventoryNumber, ProductCode, ISBN (← bridge to exercise)


### Mapping to CIDOC CRM

| Domain            | CIDOC CRM Suggestion    |
| ----------------- | ----------------------- |
| Game (content)    |          |
| Physical Copy     |          |
| Developer         |          |
| Publisher         |          |
| Release           |          |
| Platform          |          |
| Inventory Number  |          |
| ISBN/Product Code |          |


### Mini Exercise: Domain Ontology Bridge (Inventory Number vs ISBN)

Question to groups:

Are inventory numbers and ISBNs the same kind of identifier? How would you model them?

Goal:

Show difference between internal museum metadata (inventory number) and external publication metadata (ISBN/product code)

CIDOC mapping:

Both → E42 Identifier

But different property paths:

Inventory number → identity of physical item (E84 Information Carrier)

ISBN → identity of conceptual work/product (E28 Conceptual Object)


### Group Results (5 min)

Each group presents:

3–5 key entities

2–3 relationships

CIDOC mappings

Identifier distinction (inventory vs ISBN)


### Open Questions

Let's clarify open modeling questions before moving into Protégé.

