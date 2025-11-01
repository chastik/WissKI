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

Unit 2: Domain ontology modelling

From conceptual structure to semantic paths 

Duration: ~ 20 Min.

---

## Why work in draw.io?

Working in draw.io helps us, to...

* define entity classes and their roles
* express relationships as CIDOC CRM properties
* test ontology structure before implementation
* Co-model collaboratively and transparently
* communicate the domain ontology
* maintain clean and consistent semantic logic

*Based on experience, visualizations are not only a meaningful intermediate step but also an essential tool for communicating and negotiating modeling decisions. Diagrams make knowledge visible and support a shared understanding of semantic structures.*

---

## Starting Point

In Session 1, we developed the conceptual foundation of our data model:

* in **Unit 5**, we identified *core entities, relationships, and semantics* of the game domain (Zelda example)
* in **Unit 6**, we extended CIDOC CRM with *domain-specific subclasses*

---

## What we are modeling

Now we visualize this semantic model in draw.io as preparation for WissKI implementation. We start modelling the core entities and their relations semantically correct based on CIDOC CRM:

**Example results**

<table>
  <tr>
    <td><img src="../assets/Mindmap.png" alt="Conceptual Mindmap" width="75%"></td>
  </tr>
</table>

---

## Modeling requirements

* Use ontology *classes*, not instances
* Follow *CIDOC CRM mappings* 
* Use *semantic properties* (verbs) for relationships from CIDOC CRM
* reuse *domain-specific subclasses* 
* keep modeling *clean, consistent, and readable*

---

## Task (Pair Work – 15 min.)

* Open the prepared draw.io template
* Model the entities from your domain
* Use for semantic relationships CIDOC CRM properties from [CIDOC CRM specification (v7.1.3)](https://cidoc-crm.org/sites/default/files/cidoc_crm_version_7.1.3.pdf). Additional help provides the domain ontology: http://games.m-e-g-a.org/game_domain.rdf 

**Please select your group**

* Group_10: https://drive.google.com/file/d/1BR38UBlpKeWqab-fOLwndg9bxpsdu1dw/view?usp=sharing or http://tiny.cc/ISWC_10
* Group_09: https://drive.google.com/file/d/1T0imdwR-JdaVnhVTWdXJBu6h4cSU_sFk/view?usp=sharing or http://tiny.cc/ISWC_09
* Group_08: https://drive.google.com/file/d/1zfjCSq_Hfj75lZO5JR3XWeaxOJGT9flC/view?usp=sharing or http://tiny.cc/ISWC_08
* Group_07: https://drive.google.com/file/d/1-rjsKytyPnW_nUbbQ58wHDb5nKt1jxaW/view?usp=sharing or http://tiny.cc/ISWC_07
* Group_06: https://drive.google.com/file/d/1uSzcQUFZFV8Jjwb_vRrqs-FrnPxGBkyw/view?usp=sharing or http://tiny.cc/ISWC_06
* Group_05: https://drive.google.com/file/d/1BUtP_DyM-LHIkSODZwems03UjL8F8mjg/view?usp=sharing or http://tiny.cc/ISWC_05
* Group_04: https://drive.google.com/file/d/1aSlvH9FWKLg3vZdn6vI43HEbVQsXd_q0/view?usp=sharing or http://tiny.cc/ISWC_04
* Group_03: https://drive.google.com/file/d/1WhBd9XGw7KTJOzGN2nMmdvzck4kGSspL/view?usp=sharing or http://tiny.cc/ISWC_03
* Group_02: https://drive.google.com/file/d/1KsEdukcXCTc8O8JKRM4HGoB2bhxVRtfQ/view?usp=sharing or http://tiny.cc/ISWC_02
* Group_01: https://drive.google.com/file/d/1tTFWWsfsFR2QFhhmMG8QgteKfSt0JIgj/view?usp=sharing or http://tiny.cc/ISWC_01

Resources

* .pdf-file: https://cidoc-crm.org/sites/default/files/cidoc_crm_version_7.1.3.pdf
* .html-link: https://cidoc-crm.org/html/cidoc_crm_v7.1.3.html
* domain ontology: http://games.m-e-g-a.org/game_domain.rdf 

This modeling step is not just a visual exercise — the diagram is part of an (semi)automated pipeline (web-service).....

Once our domain diagrams are ready, we will transform them into WissKI Paths in the next step.







