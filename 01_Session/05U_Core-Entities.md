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

Unit 5 Identify core entities from a collection - Joint exploration.

Duration: approx. 20 Min.

### Learning Goal

In this unit, we move from theory to practice. Together, we will:

* Analyze a small domain example
* Identify core entities and relationships
* Understand the difference between domain concepts and semantic classes
* Prepare a conceptual model that we will later formalize in Protégé and WissKI

### Scenario

We will work with a sample collection of computer games inspired by the MEGA Ontology.
This example domain is ideal because it includes:

* Physical and digital objects
* Producers, creators, publishers
* Release events, platforms, versions
* Identifiers and metadata 

### Example Objects from the Collection

| Domain Element    | Example                                |
| ----------------- | -------------------------------------- |
| Game title        | *The Legend of Zelda: Ocarina of Time* |
| Release year      | 1998                                   |
| Publisher         | Nintendo                               |
| Physical copy     | Inventory number: XYZ-Museum-000123    |
| Platform          | Nintendo 64                            |
| Creator/Developer | Nintendo EAD                           |
| Contribution      | Composer: Koji Kondo                   |


Group Task

You will work in groups of 3–4 people. Your task:

| Step | Task                                                                |
| ---- | ------------------------------------------------------------------- |
| 1    | Identify **entities** in the domain (nouns: Game, Copy, Publisher…) |
| 2    | Identify **relationships** (verbs: published by, developed by…)     |
| 3    | Identify **attributes** (title, year, code…)                        |
| 4    | Map each entity to a **CIDOC CRM class**                            |
| 5    | Identify **identifier types** (inventory code, product code…)       |
| 6    | Note **domain extensions** (e.g. MEGA Ontology classes)             |

Each group will write down their findings using sticky notes or an online whiteboard.

### Modeling Focus

Before you start, please keep in mind:

| We are not yet…       | We are now…                             |
| --------------------- | --------------------------------------- |
| Building an ontology  | Creating a **conceptual domain model**  |
| Writing OWL or RDF    | Thinking about **entities and meaning** |
| Using Pathbuilder yet | Preparing content for it                |


### Group Work Brainstorming

| Step | Question                                                 | Goal                       |
| ---- | -------------------------------------------------------- | -------------------------- |
| 1    | What are we talking about?                               | Define domain and scope    |
| 2    | Which **entities** exist?                                | Identify important objects |
| 3    | Which **relationships** exist?                           | Connect entities           |
| 4    | Which **attributes** or identifiers exist?               | Domain-specific metadata   |
| 5    | How do these map to **CIDOC CRM** classes?               | Semantic grounding         |
| 6    | Which entities belong to the **domain ontology (MEGA)**? | Extend semantic meaning    |

### CIDOC CRM Mapping (Examples) - Help Table

| Domain Concept      | CIDOC CRM Suggestion              |
| ------------------- | --------------------------------- |
| Game (conceptual)   | E28 Conceptual Object             |
| Physical copy       | E84 Information Carrier           |
| Developer/Publisher | E21 Person / E74 Group            |
| Release event       | E12 Production                    |
| Platform            | E55 Type or subclass in extension |
| Inventory number    | E42 Identifier                    |
| Genre/Category      | E55 Type                          |

### Mini Exercise: Domain Ontology Bridge 

Inventory Number vs ISBN

Question to groups:

Are inventory numbers and ISBNs the same kind of identifier? How would you model them?

| Aspect      | Inventory Number        | Product Code            |
| ----------- | ----------------------- | ----------------------- |
| Purpose     | Internal museum ID      | Global commercial ID    |
| Refers to   | Physical item           | Conceptual product/work |
| CIDOC CRM   | E42 Identifier          | E42 Identifier          |
| Connects to | E84 Information Carrier | E28 Conceptual Object   |

Answer: Both are identifiers – but they identify different levels of reality.

### Output of the Group Exercise

* Each group will:
* Present 3–5 main entities
* Explain 2–3 key relationships
* Show CIDOC CRM mappings
* Discuss one modeling challenge

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






