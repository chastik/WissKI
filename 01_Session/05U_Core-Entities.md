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

Unit 4 CIDOC CRM and Domain Ontologies - Why CIDOC CRM as an underlying ontology?

Duration: approx. 10 Min.

### Learning Goal

* Identify domain core entities and relationships
* Translate inot CIDOC CRM ontology classes
* Map the classes to domain concepts to CIDOC CRM
* Prepare a shared conceptual model for later semantic modeling
* Recognize the role of domain ontologies (e.g. MEGA Ontology)

### Setup

* Method: Group work (3–4 people per group)
* Material: Sticky notes or small cards + pens OR Etherpad/Miro / Laoptop
* Example domain: Computer game collection (based on MEGA ontology example)

### Your Task

In groups you analyze a small collection scenario and identify the key entities and relationships of the domain. 

Your results are part of the conceptual foundation for our later semantic modeling in Protegé (Unit 5) and WissKI (Session 2). 

Each group will collaboratively build a part of the domain model and briefly present the results.

### Example Objects from the Collection

| Kategorie            | Information                                   | Bild                                                |
| -------------------- | --------------------------------------------- | --------------------------------------------------- |
| **Game**             | *The Legend of Zelda: Ocarina of Time* (1998) | ![Bildplatzhalter]() |
| **Physische Kopie**  | Museumsexemplar mit Inventarnr. **xxxxxxx**   | ![Bildplatzhalter]() |
| **Publisher**        | Nintendo                                      | ![Bildplatzhalter]() |
| **Plattform**        | Nintendo 64                                   | ![Bildplatzhalter]() |
| **Entwickler**       | Nintendo EAD                                  | ![Bildplatzhalter]() |
| **Veröffentlichung** | 1998 in Japan                                 | ![Bildplatzhalter]() |

### The Scenario

A museum holds a collection of computer games. 

Each game has a title, release year, and publisher. 

The museum keeps physical copies of the games, which are stored under inventory numbers. 

Some games have contributors such as designers and composers. 

Games are released on one or more platforms and exist as physical versions.


### Group Work Brainstorming

| Step | Question                                                 | Goal                       |
| ---- | -------------------------------------------------------- | -------------------------- |
| 1    | What are we talking about?                               | Define domain and scope    |
| 2    | Which **entities** exist?                                | Identify important objects |
| 3    | Which **relationships** exist?                           | Connect entities           |
| 4    | Which **attributes** or identifiers exist?               | Domain-specific metadata   |
| 5    | How do these map to **CIDOC CRM** classes?               | Semantic grounding         |
| 6    | Which entities belong to the **domain ontology (MEGA)**? | Extend semantic meaning    |


### Clarification – What are we modeling here?

In this unit, we are not building an ontology yet.

We are conceptualizing part of a domain by describing entities and relationships.

The output is an extension of a domain model – a structured understanding of your collection.

This extension will be formalized later in Protégé (ontology) and implemented in WissKI.

The MEGA ontology is used as inspiration and vocabulary support, not as a constraint.

### CIDOC CRM Mapping (Examples)

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


### Mini Exercise: Domain Ontology Bridge 

Inventory Number vs ISBN

Question to groups:

Are inventory numbers and ISBNs the same kind of identifier? How would you model them?

|             | Inventory Number               | ISBN/Product Code             |
| ----------- | ------------------------------ | ----------------------------- |
| Purpose     | Internal museum identification | Global publication/product ID |
| Applies to  | Physical copy                  | Conceptual work or edition    |
| CIDOC Class | E42 Identifier                 | E42 Identifier                |
| Linked to   | **E84 Information Carrier**    | **E28 Conceptual Object**     |


Goal:

Show difference between internal museum metadata (inventory number) and external publication metadata (ISBN/product code)

CIDOC mapping:

Both → E42 Identifier

But different property paths:

Inventory number → identity of physical item (E84 Information Carrier)

ISBN → identity of conceptual work/product (E28 Conceptual Object)


### Group Results (5 min)

Each group presents:

* 3–5 key entities
* 2–3 relationships
* CIDOC mappings
* Identifier distinction (inventory vs ISBN)

### Open Questions

Let's clarify open modeling questions before moving into Protégé.

(Übergang zu Unit 5, we will formalize your domain concepts as classes and relationships using Protégé.)





