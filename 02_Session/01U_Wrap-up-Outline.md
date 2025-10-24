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

# Develop and implement your data model 

Develop and implement your data model

From diagram to paths - applying and …

Unit 1 Wrap-up:  Short retrospective of Session 1

Duration: approx. 5 Min.

### What We Will Do in Session 2

Now we move from conceptual modeling to implementation.

| From              | To                                |
| ----------------- | --------------------------------- |
| Diagram           | Semantic Paths                    |
| Modeling on paper | Modeling in draw.io               |
| Domain logic      | Ontology structure                |
| Conceptual model  | WissKI Pathbuilder implementation |


In Session 1, we built the conceptual foundation for our data model:

* We explored the workflow from data to semantics
* We learned how CIDOC CRM provides structure and meaning
* We identified core entities and relationships in a domain example
* We mapped them conceptually using domain modeling methods
* We discussed semantic clarity vs. practical modeling decisions

In short: Session 1 was about understanding and modeling meaning.

### Tutorial Outline - Session 2

* Unit 1 Wrap-up (5 Min.)
  
  Short retrospective of Session 1 and transition to implementation phase.
  
* Unit 2 Domain ontology modelling (20 Min.)
  
  Entity mapping and semantic structuring in draw.io based on the domain perspective.
  
* Unit 3 From draw.io to WissKi Pathbuilder (20 Min.)
  
  Translating the conceptual model into implementation paths using the WissKI Pathbuilder and the FORTH-ICS web service.
  
* Unit 4 Where is WissKI heading?  (10 Min.)
  
  Outlook on current developments, extension concepts, and future requirements.
  
* Unit 5 Q&A and takeaways (15 Min.)
  
  Participants provide feedback on the workflow, reflect on modeling decisions, and discuss strategies for applying semantic structures in their own data context.
  
* Unit 6 Farewell and feedback (15 Min.)
  
  Summary of key insights and closing meta-reflection on knowledge transfer and practical implementation.



### From Draw.io to Pathbuilder Pipeline

Once you have your domain ontology you can follow a hands-on workflow:

* Step 1: Design semantic entity diagram in draw.io
* Step 2: Parses draw.io diagrams according to a json configuration file
* Step 3: Identifies specific paths originating from a central node
* Step 4: Applies syntactic validation of these paths against a set of online ontology files specified in the json configuration file
* Step 5: Exports the identified ontology paths to a Pathbuilder XML file.

We begin with domain ontology modeling in draw.io to structure our entities before implementation.

✅ Ready to start? Then let’s continue with Unit 2 – Domain Ontology Modeling in draw.io.


