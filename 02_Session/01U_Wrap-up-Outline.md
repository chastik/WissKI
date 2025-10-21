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

From diagram to paths - applying and xxxx evaluating?

### Wrap-up Session 1

* Introduced ontology-driven data modeling and the goals of the tutorial
* Explored WissKI as a semantic research environment for GLAM data
* Understood the role of CIDOC CRM for semantic structuring and context
* Discussed the workflow from data analysis → conceptual modeling → ontology mapping
* Group activity: identified domain entities, relationships, and identifiers
* Mapped domain concepts to CIDOC CRM classes and properties
* Clarified the difference between conceptual objects vs. physical items
* First insights into ontology extension using Protégé (MEGA ontology example)
* Reflected on modeling challenges and key questions for implementation in WissKI


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

once you have your domain ontology... 

* Step 1: Design semantic entity diagram in draw.io
* Step 2: Parses draw.io diagrams according to a json configuration file
* Step 3: Identifies specific paths originating from a central node
* Step 4: Applies syntactic validation of these paths against a set of online ontology files specified in the json configuration file
* Step 5: Exports the identified ontology paths to a Pathbuilder XML file.  




