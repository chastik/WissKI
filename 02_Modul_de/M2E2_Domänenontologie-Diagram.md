<!--

icon: https://raw.githubusercontent.com/chastik/Beratung_Dateityp_Bild/refs/heads/main/SODa-Logo_full.svg
link: https://raw.githubusercontent.com/chastik/Beratung/refs/heads/main/soda.css

-->

# SODa WissKI Bits 

**Modul 2 DATENMODELL ENTWICKELN UND IMPLEMENTIEREN AM BEISPIEL** 

Vom Diagramm zu Pfaden – Erläutern und anwenden

Einheit 2: **Visualisierung eines Domänenontologie-Diagramms**  

**Dauer:** ~ 25 Min.

---

## Warum in Draw.io arbeiten?

Visualisierungen sind ein bedeutender Zwischenschritt und ein wesentliches Werkzeug, um Modellierungsentscheidungen zu kommunizieren, auszuhandeln und ein gemeinsames Verständnis über semantische Strukturen zu fördern.

Dieser Modellierungsschritt ist nicht nur eine visuelle Übung – das Diagramm ist Vorraussetzung für die (halb-)automatisierten Pipeline zur Herstellung eines Pathbuilders in WissKI. 


**Draw.io hilft uns dabei…**

* Entitätsklassen und ihre Beziehungen festzulegen.
* kollaborativ und transparent gemeinsam zu modellieren.
* die Domänenontologie und die Logik sichtbar zu machen und zu diskutieren.
* die Ontologiestruktur vor der Implementierung zu testen.  

---

## Ausgangspunkt

In Modul 1 haben wurde die konzeptionelle Grundlage unseres Datenmodells entwickelt:

* In **Einheit 5** sind *zentralen Entitäten und Beziehungen* einer Beispiel-Domäne identifiziert.  
* In **Einheit 6** wurde die Top-Level Ontologie CIDOC CRM um *domänenspezifische Subklassen* erweitert.  

### Datenbeispiel

**Beispielobjekt**

Super Nintendo Entertainment System (SNES) Spiel: *The Legend of Zelda*

| Darstellung | Beschreibung |
|------------|--------------|
| **Objekt** | ![Zelda Spiel](../assets/zelda_smal.png) |
| **Semantische Annahme** | Titel des Objekts: *The Legend of Zelda: A Link to the Past* |
| **Draw.io Modell** | ![draw.io Diagramm](../assets/path.PNG) |
| **WissKI Pathbuilder** | ![WissKI Pathbuilder](../assets/pathbuilder.PNG) |

**Beispiele für Spielmerkmale**

* Plattform (z. B. Nintendo 64, PlayStation, PC)
* Genre (z. B. Action-Adventure, RPG)
* Edition oder Version (z. B. Collector’s Edition, Remastered)

**Beispiele für narrative Elemente**

* Perspektive (z. B. First-Person, Third-Person)
* Spielbeschreibung
* Charaktere / Figuren

---

## Was wir modellieren

Modelliert wird das semantische Modell in Draw.io als Grundlage für die Erstellung von Pfaden im WissKI Pathbuiler.  
Hierfür werden die Kernentitäten und ihre Beziehungen der Beispieldomäne semantisch korrekt auf Basis des CIDOC CRM visualisiert:

**Beispielergebnisse**

<table>
  <tr>
    <td><img src="../assets/Mindmap.png" alt="Konzeptionelle Mindmap" width="75%"></td>
  </tr>
</table>

---

## Anforderungen an das Arbeiten mit Draw.io

* Es werden keine individuelle Instanzen abgebildet.
* Es werden die domänenspezifischen Sub-Klassen aus der bereits erstellten Domänenontologie verwendet.
* Die semantischen Relationen sind aus CIDOC CRM abzuleiten.
* Es sind vollständige Pfade zu erstellen.
* Dem zentralen Startknoten, jedem Gruppenknoten und jedem Blattknoten werden jeweils **element_id**, **group_name** und **name** zugewiesen.  

---

## Aufgabe (Partnerarbeit – 20 Min.)

* Öffnet die vorbereitete Draw.io-Vorlage (siehe Gruppen)
* Vervollständigt das Diagramm   
* Nutzt für semantische Beziehungen die CIDOC CRM-Properties aus der [CIDOC CRM-Spezifikation (v7.1.3)](https://cidoc-crm.org/sites/default/files/cidoc_crm_version_7.1.3.pdf).
* Nutzt für die Domänenspezifischen Subklassen den bestehenden [.rdf-Entwurf](http://games.m-e-g-a.org/game_domain.rdf).

**Für Anfänger**

* Gruppe 15: http://tiny.cc/WAT-Gruppe_15
* Gruppe 14: http://tiny.cc/WAT-Gruppe_14
* Gruppe 13: http://tiny.cc/WAT-Gruppe_13
* Gruppe 12: http://tiny.cc/WAT-Gruppe_12
* Gruppe 11: http://tiny.cc/WAT-Gruppe_11
* Gruppe_05: http://tiny.cc/WAT-Gruppe_5
* Gruppe_04: http://tiny.cc/WAT-Gruppe_04
* Gruppe_03: http://tiny.cc/WAT-Gruppe_03
* Gruppe_02: http://tiny.cc/WAT-Gruppe_02
* Gruppe_01: http://tiny.cc/WAT-Gruppe_01


**Für Experten** 

* Gruppe_10: http://tiny.cc/WAT-Experts_10
* Gruppe_09: http://tiny.cc/WAT-Experts_09
* Gruppe_08: http://tiny.cc/WAT-Experts_08
* Gruppe_07: http://tiny.cc/WAT-Experts_07
* Gruppe_06: http://tiny.cc/WAT-Experts_06 

---

### Ressourcen

* **PDF-Datei:** [https://cidoc-crm.org/sites/default/files/cidoc_crm_version_7.1.3.pdf](https://cidoc-crm.org/sites/default/files/cidoc_crm_version_7.1.3.pdf)  
* **HTML-Link:** [https://cidoc-crm.org/html/cidoc_crm_v7.1.3.html](https://cidoc-crm.org/html/cidoc_crm_v7.1.3.html)  
* **Domänenontologie:** [http://games.m-e-g-a.org/game_domain.rdf](http://games.m-e-g-a.org/game_domain.rdf)

---












