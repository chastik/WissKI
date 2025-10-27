
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

<table>
  <tr>
    <td><img src="../assets/gnm.jpg" alt="GNM" width="75%"></td>
    <td><img src="../assets/gnm_2.JPG" alt="GNM" width="75%"></td>
  </tr>
</table>

WissKI is not just a database for exhibitions and collections - it is a semantic data management system and enables researchers to model data semantically als Linked Open Data (LOD) and make it interoperable and FAIR (Findable, Accessible, Interoperable, Reusable)

## WissKI Modules in Drupal 10

WissKI...

* is built as a **semantic extension of Drupal 10**
* consists of **interoperating Drupal modules**
* **is not a standalone system**
* stores data **natively in RDF triple stores (SPARQL 1.1)**
* inherits Drupal core features:
  * **User and role management**
  * **Multilingual support**
  * **REST/JSON APIs**
  * **Security and access control**
  * **Modular extensibility**
* adds semantic capabilities:
  * **CIDOC CRM integration**
  * **OWL-based ontology support**
  * **Pathbuilder for semantic paths**
  * **Linked Open Data publishing**

<table>
  <tr>
    <td><img src="../assets/wisski_architektur.png" alt="GNM" width="75%"></td>
  </tr>
</table>


## WissKI Key Features 

* Semantic Paths

Instead of traditional database tables, WissKI uses semantic paths based on ontology properties.

* Pathbuilder

A modeling tool inside WissKI that lets you define your data structure without writing code.

* Entity Management

Supports structured handling of People, Places, Events, Objects, and more.

* Ontology Integration

Compatible with CIDOC CRM and other domain ontologies.

* SPARQL Endpoint

Data can be queried using SPARQL and shared as Linked Open Data.

* Modular System

Built as modules on top of Drupal CMS.


## The WissKI Pathbuilder

The Pathbuilder is the heart of WissKI and defines the semantic data model.



* Groups (semantic entity types)
* Paths (semantic connections between entities)
* Widgets/forms for data entry

This allows us to model meaning while providing user-friendly forms for data input.

## Semantic Data Modeling (the WissKI-Way)






____________________________________________________________________________________________Reste_____________________________
In a traditional database, you would model tables and fields.
In WissKI, you model entities and relationships—the semantic meaning of your data.

Object → was created by → Person → in → Production Event → at → Place

These relationships are meaningful, reusable, and interoperable.

From Ontology to Implementation

WissKI uses ontologies not only for annotation but as a structural backbone.
Semantic relationships become paths, and paths become forms.

This creates a transparent connection between:

Conceptual modeling (ontology)

Implementation (Pathbuilder)

Data entry (Bundles & Fields)

Knowledge graph output (RDF)

This is the foundation for the hands-on work we will begin later: building our own semantic paths and forms based on domain logic.

Now that we understand how WissKI builds on semantic modeling, we will look at the ontology behind our models: CIDOC CRM.

Konstruktion
aus ontologien werden Pfade aus Pfaden ... Seite 3 .pdf 
theorestisch als Sceenshot evtl. auch in WissKI selbst...

Motivation für draw.io: mehr semantic modelling statt pahtbuilding :)

Ontologie Thema teasern






