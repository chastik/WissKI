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

##  Live Demo in Protegé

This session introduces the conceptual process of extending an existing MEGA domain ontology using Protégé.

I will show you briefly how to build and extend an ontology while preserving semantic clarity.

The focus is on methodology, ontology engineering principles, and clean integration strategies.

### Live Demo – Overview of Steps

* open Protégé and load an existing ontology (e.g. CIDOC CRM)
* explore ontology structure (classes, object properties, data properties)
* create **subclasses** for new domain concepts (e.g. `Game_Characteristic`, `Platform_Type`, `Genre_Type`, `Edition_Type`)
* define **class hierarchy** and attach **rdfs:labels** and **definitions**
* add **CIDOC CRM alignment** using `rdfs:subClassOf` mappings
* model **object properties** according to the semantic paths (e.g. `hasPlatform`, `hasGenre`)
* add **restrictions / domains / ranges** to ensure clean modeling
* annotate classes and properties with **documentation and provenance**
* check for **reasoning consistency** using the Protégé reasoner
* save and export the extended ontology module




