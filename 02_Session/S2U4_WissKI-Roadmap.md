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

**DEVELOP AND IMPLEMENT YOUR DATA MODEL** 

From diagram to paths - explaining and applying

Unit 4: Where is WissKI heading? 

Duration: ~ 10 Min.

---

## From semantic paths to interaction

In Unit 3, we generated semantic paths using the Pathbuilder pipeline.  

However, paths alone are not visible in the user interface. 

To make WissKI usable for data entry, we need:

* **Bundles** – logical groupings of semantic paths
* **Fields** – input components that connect paths to widgets

These elements transform the semantic model into a practical research environment.

---

## What are Bundles?

A **Bundle** groups related semantic paths and represents a logical section of a data entry form in WissKI.

* groups related information for one entity
* structures input on forms
* improves usability

**Example: Bundle – Game Metadata**

| Path | Description |
|------|-------------|
| Computer_Game → P102 has title → E35 Title → P190 has symbolic contend →  Literal | title | 
| Computer_Game → P94 was created by → E65 Creation → P14 carried out by → E74 Group | developer |
| Computer_Game → P129 is about → Game_Characteristic | characteristics |

---

## What are Fields?

A **Field** defines how a semantic path is displayed and edited in a WissKI form.

* connects a semantic path to a widget
* defines input types (text, date, autocomplete, dropdown)
* enables validation and controlled data entry

| Path | Field type |
|------|------------|
| has title | text field |
| release year | date picker |
| game genre | controlled vocabulary dropdown |
| developer | entity reference autocomplete |

---

## Why Bundles and Fields matter

Without Bundles and Fields:

* paths are invisible
* editors cannot enter data
* no user interface exists

With Bundles and Fields:

* the semantic model becomes usable
* custom data entry interfaces are created
* research data can be entered consistently

---

## Optional WissKI Demonstration

A short demo at this stage can help illustrate the goal:

* open an existing WissKI instance
* show how semantic paths generate input forms
* display entity connections (linked data)
* run a simple SPARQL query

(https://portal.m-e-g-a.org/)

---

### SPARQL

Link: https://portal.m-e-g-a.org/wisski/endpoint/backend/

>
>SELECT * WHERE { ?s ?p ?o } LIMIT 10
>

>
>SELECT * WHERE { GRAPH ?g { ?s ?p ?o }} LIMIT 10
>

>
>SELECT * WHERE { GRAPH ?g { ?s ?p ?o } . FILTER(CONTAINS(?o, "Zelda"))} LIMIT 10
>

>
>SELECT * WHERE { GRAPH ?g { ?s ?p ?o } . FILTER(CONTAINS(?o, "Zelda"))} ORDER BY ASC(?o)
>



