
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

**DEVELOP AND IMPLEMENT YOUR DATA MODEL**

From collection to diagram - understanding and explaining

**Unit 3:  WissKI in a nutshell - Short introduction to WissKI and its architecture**

Duration: ~ 5 Min.

---

## WissKI in a Nutshell

WissKI (Wissenschaftliche Kommunikations-Infrastruktur) is:

* a free, open-source virtual research environment
* designed for cultural heritage and research data
* based on semantic web technologies
* modular and standards-based

WissKI is used at the Germanisches Nationalmuseum (GNM) in Nuremberg,

* the largest cultural history museum in the German-speaking world
* setting standards in digital research infrastructure

WissKI is not just a collection database – it is a semantic data management system for Linked Open Data (LOD) following the FAIR principles
(Findable, Accessible, Interoperable, Reusable).

<table>
  <tr>
    <td><img src="../assets/gnm.jpg" alt="GNM" width="75%"></td>
    <td><img src="../assets/gnm_2.JPG" alt="GNM" width="75%"></td>
  </tr>
</table>

---

## WissKI and Drupal 10

WissKI is not a standalone application. It is built as a semantic extension of Drupal 10.

<table>
  <tr>
    <td><img src="../assets/drupal.JPG" alt="wisski" width="75%"></td>
  </tr>
</table>


| Drupal provides ...    | WissKI adds ...                   |
| ---------------------- | --------------------------------- |
| User & role management | Semantic modeling with ontologies |
| Modular framework      | Pathbuilder for semantic paths    |
| REST & JSON APIs       | RDF-native triple store           |
| Access control         | SPARQL endpoint                   |
| Multilingual interface | Linked Open Data publishing       |

---

## The WissKI Pathbuilder

The Pathbuilder is the heart of WissKI.

Instead of tables, WissKI uses ontology-based structures.

It defines:

* Groups → semantic entity types, e.g. Object, Person, Place, Event
* Paths → semantic relations from ontologies, e.g. Object → created by → Person
* Widgets → automatically generated data entry forms, where form logic follows semantic relations

This keeps WissKI structured, flexible, and enables ontology-based modeling keeping the user interface simple and practical.

**Screenshot**

<table>
  <tr>
    <td><img src="../assets/pathbuilder.jpg" alt="Pathbuilder" width="75%"></td>
  </tr>
</table>

---

## Semantic Modeling the WissKI-Way

In WissKI, we don’t just store data – we model **meaning**.

In WissKI we ask:<br>
> *What is the real-world relationship between an object and a person?*

!?[autoplay video](../assets/semanticModelling.mp4)

The video demonstrates how knowledge is connected step by step:

* Albrecht Dürer → Person
* was born in → Place (Nuremberg)
* at → Time-span
* had a mother → Person
* created → Self-Portrait (Object)
* during → Career period
* in → Nuremberg

Multiple facts connect into a semantic graph. Different sources merge into one consistent network of knowledge.

---

## Benefits of WissKI

* Enables semantic knowledge representation instead of rigid table structures
* Ensures interoperability through established ontologies such as CIDOC CRM
* Follows the FAIR principles (Findable, Accessible, Interoperable, Reusable)
* Provides automatically generated data entry forms based on semantic paths
* Facilitates publication as Linked Open Data (LOD)
* Offers powerful querying through SPARQL
* Combines conceptual clarity with technical implementation

---

WissKI embeds semantic logic at the core of data management:

* CIDOC CRM ontology – defines domain concepts and their interrelations
* Semantic paths – map logical data structures within the Pathbuilder
* Forms and data entry – enforce consistent schema-based knowledge input
* RDF knowledge graph – provides a standards-compliant backbone for data exchange and Linked Open Data publication






















