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

# SODa WissKI-ISWC25 Bits

Develop and implement your data model 

From collection to diagram - understanding and explaining

Unit 3 From draw.io to WissKi Pathbuilder 

Duration: approx. 20 Min.

## Why this step matters?

In draw.io, we modeled semantic relationships.

But WissKI needs semantic paths to structure data entry and the RDF graph.

So we now translate ontology relations into WissKI Paths.

This step builds the bridge from modeling to implementation.

## From ontology to paths

Conceptual modeling focuses on classes and relations.

WissKI needs paths, which are chains of ontology properties that describe how entities are connected.

Example:

Ontology relation:

Game → was produced by → Production Event → carried out by → Group

WissKI Path version:

Game → P94 was created by → Production Event
     → P14 carried out by → Group

Each row becomes a Path in the WissKI Pathbuilder.

## What is the Pathbuilder?

The WissKI Pathbuilder is a modeling tool inside WissKI where we define:

| Term       | Meaning                                               |
| ---------- | ----------------------------------------------------- |
| **Group**  | An entity type (e.g. Game, Person, Release Event)     |
| **Path**   | A sequence of ontology properties connecting entities |
| **Domain** | CIDOC CRM (or domain ontology)                        |
| **Range**  | Target class of a Path                                |

WissKI uses these to generate form logic and RDF data structure.

## Pipeline: draw.io → WissKI XML

To save time, we use the MEGA Pathbuilder Pipeline, developed with FORTH-ICS.
This pipeline can automatically convert draw.io ontology diagrams into WissKI Pathbuilder XML files.

* No manual clicking in Pathbuilder
* Reusable semantic model
* Consistent ontology grounding

Pipeline Workflow

| Step | Action                               |
| ---- | ------------------------------------ |
| 1    | Export draw.io model as `.xml`       |
| 2    | Upload to pipeline service           |
| 3    | Pipeline verifies ontology structure |
| 4    | Generates **WissKI Pathbuilder XML** |
| 5    | Import XML into WissKI               |
| 6    | Paths appear automatically           |

## Hands-on Task (Pair work – 15 min)

Using the diagram you built in Unit 2:

* Export your draw.io file (.xml)
* Upload it to the Pathbuilder pipeline
* Generate the Pathbuilder XML
* Inspect the created semantic paths
* Download and prepare for import in Unit 4

Now we have a Pathbuilder XML based on your domain model.
