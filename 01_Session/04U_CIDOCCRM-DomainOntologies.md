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

## Why CIDOC CRM?

* ISO standard ontology for cultural heritage
* Models events, actors, objects, time, and space
* Focuses on context and provenance
* Widely used in DH and GLAM
* WissKI is based on OWL ontologies and can also use others

## Key CIDOC CRM Concepts (Basic Vocabulary)

| Concept Type | Example Class       |
| ------------ | ------------------- |
| Person       | E21 Person          |
| Group        | E74 Group           |
| Event        | E5  Event           |
| Place        | E53 Place           |
| Time         | E52 Time-Span       |

## CIDOC CRM theoretisch und praktisch 

Ausgehend von E1
Trägerontologie als Mehrwert
alles leitet sich vom top level modell ab
dann CIDOC CRM Struktur - an hand eines Beispiels zeigen

Quelle VErlinken


##  Example Knowledge Graph

*A vase was found during an excavation by a research team in Nara in 2005.*

E22 Object → was found by → E5 Event → carried out by → E74 Group
                          
E22 Object → took place at → E53 Place
                          
E22 Object → occurred in → E52 Time-Span


Erweitern: Top ontologies vs domain ontologies



Now that we understand the logic behind WissKI and CIDOC CRM, we will start applying it. In the next unit, we begin modeling our first data entities step by step.

