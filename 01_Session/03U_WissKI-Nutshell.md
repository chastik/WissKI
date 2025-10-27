
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

# SODa WissKI-ISWC25 Bits

DEVELOP AND IMPLEMENT YOUR DATA MODEL

From collection to diagram - understanding and explaining

**Unit 3:  WissKI in a nutshell - Short introduction to WissKI and its architecture**

Duration: ~ 15 Min.

## WissKI in a Nutshell

WissKI...

* stands for "Wissenschaftliche Kommunikations-Infrastruktur" (Scientific Communication Infrastructure) 
* is an open-source, free, web-based virtual research environment for scientific research and cultural heritage data
* based on the Wiki-approach
* is modular and flexible supporting many standards and interfaces.

WissKI is used in the **Germanisches Nationalmuseum**, the largest museum of cultural history in the German-speaking region. Setting nation-wide standards through its scientific and scholarly achievements.

WissKI is not just a database for exhibitions and collections - it is a semantic data management system and enables researchers to model data semantically als Linked Open Data (LOD) and make it interoperable and FAIR (Findable, Accessible, Interoperable, Reusable).

<table>
  <tr>
    <td><img src="../assets/gnm.jpg" alt="GNM" width="50%"></td>
    <td><img src="../assets/gnm_2.JPG" alt="GNM" width="50%"></td>
  </tr>
</table>



## WissKI Modules in Drupal 10

WissKI...

* is not a standalone system
* is built as a semantic extension of Drupal 10
* consists of interoperating Drupal modules
* stores data natively in RDF triple stores (SPARQL 1.1)

<table>
  <tr>
    <td><img src="../assets/drupal.jpg" alt="wisski" width="100%"></td>
  </tr>
</table>


| Drupal provides …                        | WissKI adds …                               |
|------------------------------------------|---------------------------------------------|
| User and role management                 | Semantic modeling with ontologies           |
| Modular framework                        | Pathbuilder for semantic paths              |
| REST and JSON APIs                       | RDF-native triple store                     |
| Access control and security              | SPARQL endpoint                             |
| Multilingual interface                   | Linked Open Data publishing                 |


## The WissKI Pathbuilder

The Pathbuilder is the heart of WissKI and defines the semantic data model.

Instead of designing tables like in a relational database, WissKI uses ontological logic to structure data.

The Pathbuilder defines:

* Groups - semantic entity types (e.g. Object, Person, Place, Event)
* Paths – semantic relationships based on an ontology (e.g. “Object → created by → Person”)
* Widgets/forms – data entry interfaces automatically generated from paths

This enables ontology-based modeling keeping the user interface simple and practical.

## Semantic Data Modeling (the WissKI-Way)

In WissKI, we don’t just store data – we model **meaning**.

In a traditional database you ask:<br>
> *Which table stores persons and how do I join them to objects?*

In WissKI we ask:<br>
> *What is the real-world relationship between an object and a person?*

Example semantic expression:

**Object → was produced by → Production Event → carried out by → Person → at → Place**

!?[autoplay video](../assets/semanticModelling.mp4)

WissKI connects **conceptual modeling** with **technical implementation** in a transparent way:

| Step | Description |
|------|-------------|
| **Ontology** | Defines the domain knowledge using classes (e.g. *E22 Man-Made Object*) and relationships (e.g. *P108 was produced by*) from CIDOC CRM or other ontologies. This step captures the **semantic meaning** of the data. |
| **Pathbuilder** | Translates the ontology into **semantic paths**. These paths represent meaningful relationships between concepts and form the **data model** inside WissKI. No tables or SQL schemas are needed. |
| **Form generation** | Based on path definitions, WissKI automatically creates **data entry forms** (bundles). These forms follow the semantic logic of the ontology and ensure consistent, structured data input. |
| **Knowledge graph** | The entered data is stored as **RDF triples** and can be queried and published via **SPARQL** or exported as **Linked Open Data** — making the data reusable beyond WissKI. |

## WissKI Benefits

* WissKI uses semantic data modeling to create meaningful, machine-readable relationships between data instead of relying on technical table structures.
* Semantic relationships reflect real-world meaning and enable consistent knowledge representation.
* Ontologies like CIDOC CRM provide the conceptual foundation for modeling entities and their relationships.
* The WissKI Pathbuilder translates ontology logic into semantic paths that form the internal structure of the data model.
* These semantic paths are used to automatically generate data entry forms (bundles) that follow ontology logic instead of fixed database schemas.
* Entered data is stored as RDF triples and can be queried or published as Linked Open Data through SPARQL.
* This makes WissKI data interoperable across projects and institutions and supports long-term reuse beyond a single system.
* The approach follows the FAIR principles: Findable, Accessible, Interoperable, and Reusable.

WissKI connects conceptual modeling with technical implementation in a transparent way:

  Ontology (concepts and relations)  
  ↓  
  Semantic paths in WissKI (Pathbuilder)  
  ↓  
  Forms and data input (Bundles)  
  ↓  
  RDF knowledge graph (Linked Open Data)













