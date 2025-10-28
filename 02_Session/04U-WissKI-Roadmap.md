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

Unit 4 Where is WissKI heading? Outlook on current developments, extension concepts, and future requirements.

Duration: approx. 10 Min.

## From Paths to Data Entry

In the previous unit, we created semantic paths using the Pathbuilder pipeline.
However, paths alone do not create a usable interface.

To actually enter data in WissKI, we need Bundles and Fields.

This unit explains what they are and how we prepare WissKI for hands-on data entry.

## What are Bundles?

In WissKI, a Bundle groups related semantic paths into a logical data entry unit.

A bundle represents one aspect of an entity

It defines which fields exist on a data entry form

You can think of it like a form section

Example: Bundle for Game

| Path                                      | Description |
| ----------------------------------------- | ----------- |
| Game → has title → Literal                | Title       |
| Game → was released in → Production Event | Release     |
| Game → was created by → Group             | Developer   |

## What are Fields?

Fields define how a path is displayed and edited in the user interface.

They connect paths to widgets

They define input types (text, date, dropdown, link)

They improve data quality and usability

| Path         | Field Type                     |
| ------------ | ------------------------------ |
| has title    | Text field                     |
| release year | Date picker                    |
| genre        | Controlled vocabulary dropdown |
| developer    | Entity reference autocomplete  |

## Why this matters

Without Bundles and Fields:

Paths are invisible

Editors cannot enter data

The system has no UI

With Bundles and Fields:

* Semantic model becomes practical
* Real datasets can be entered
* Usability increases

Example – From Path to Bundle

Path:
Game → P102 has title → Literal

Becomes a Field in a Bundle:

Bundle Name: Game Description
Field: Title (Text Input)


## Hands-On in Next Step

In the next unit, you will:

* Import your Pathbuilder XML
* Create Bundles and Fields
* Build your first WissKI data entry form


## Transition

We now move from semantic structure to practical implementation.
Get ready to open your WissKI instance.
