<!--

icon: https://raw.githubusercontent.com/chastik/Beratung_Dateityp_Bild/refs/heads/main/SODa-Logo_full.svg
link: https://raw.githubusercontent.com/chastik/Beratung/refs/heads/main/soda.css

-->


# SODa WissKI-ISWC25 Bits

**DEVELOP AND IMPLEMENT YOUR DATA MODEL** 

From diagram to paths - explaining and applying

Unit 4: Where is WissKI heading? 

Duration: ~ 10 Min.

---

## From semantic paths to interaction

In Unit 3, we created semantic paths using the Pathbuilder pipeline.

However, these paths by themselves are not directly visible in the user interface.

To make WissKI functional for data entry, we must define:

* Bundles – logical groupings that organize related semantic paths
* Fields – input components that link paths to user interface widgets

Together, these elements turn the underlying semantic model into a usable and interactive research environment.

---

## What are Bundles?

A Bundle organizes related semantic paths into a coherent unit, representing a logical section of a data entry form in WissKI.

A Bundle... 

* is a Drupal content type
* it defines a semantic container for a certain kind of entity (e.g., Person, Object, Place).
* collects semantic paths that describe that entity.
* correspond to forms used for data entry and editing.

**Example: Bundle – Game Metadata**

| Path | Description |
|------|-------------|
| Computer_Game → P102 has title → E35 Title → P190 has symbolic contend →  Literal | title | 
| Computer_Game → P94 was created by → E65 Creation → P14 carried out by → E74 Group | developer |
| Computer_Game → P129 is about → Game_Characteristic | characteristics |

---

## What are Fields?

A Field defines how a semantic path is displayed and edited in a WissKI form.

A Field...

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

## Why Bundles and Fields matter?

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





