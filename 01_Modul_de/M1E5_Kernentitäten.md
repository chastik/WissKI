<!--

icon: https://raw.githubusercontent.com/chastik/Beratung_Dateityp_Bild/refs/heads/main/SODa-Logo_full.svg
link: https://raw.githubusercontent.com/chastik/Beratung/refs/heads/main/soda.css

-->

# SODa WissKI-ISWC25 Bits

**ENTWICKELN UND IMPLEMENTIEREN SIE IHR DATENMODELL** 

Von der Sammlung zum Diagramm – verstehen und erklären

---

## Einheit 5: Kerneinheiten einer Sammlung identifizieren  

**Übung - Exploration**  

**Dauer:** ~ 20 Min.

---

## Ziel und Szenario

Dies ist eine Praxiseinheit.

Ausgehend von unserem Beispiel **„Zelda“** sollen **Kernkonzepte** benannt werden, die Eigenschaften des Spiels bzw. von Spiele im Allgemeinen beschreiben. 

Ziel ist es, eine **bestehende Domänenontologie für Computerspiele zu erweitern**.

Vorgehen:

* die Beispiel-Domäne (Computerspiele) analysieren
* **Kerneinheiten** (Entitäten) und **bedeutsame Beziehungen** identifizieren
* Konzepte **CIDOC CRM-Klassen und -Eigenschaften zuordnen**
* ein erstes **konzeptionelles Datenmodell (Mindmap)** vorbereiten, das später in **Protégé** formalisiert und in **WissKI** importiert wird.

---

## Warum diese Domäne?

Die Domäne **Computerspiele** eignet sich gut für semantische Modellierung, weil sie...:

* sowohl **physische** als auch **digitale** Objekte umfasst.
* **reiche Produktions- und Veröffentlichungskontexte** enthält (Studios, Teams, Publisher).
* **Ereignisstrukturen** abbildbar macht (z. B. Release-Events).
* **Versionen, Editionen und Adaptionen** berücksichtigt.
* **persistente Identifikatoren** verwendet.
* sowohl **deskriptive** als auch **funktionale** Metadaten beinhaltet.

---

## Fokus der Erweiterung

* **Spieltitel**
* **Spielmerkmale (characteristics)**
* **Narrative bzw. erzählerische Elemente**

---

### Beispiele für Spielmerkmale

* Plattform (z. B. Nintendo 64, PlayStation, PC)
* Genre (z. B. Action-Adventure, RPG)
* Edition oder Version (z. B. Collector’s Edition, Remastered)

---

### Beispiele für narrative Elemente

* Perspektive (z. B. First-Person, Third-Person)
* Spielbeschreibung
* Charaktere / Figuren

---

## Gruppenarbeit

Gruppen von **2–4 Personen**, erarbeiten ein **konzeptionelles Modell** der Domäne auf (digitalem) Papier.

**Aufgabe:**

* **Kerneinheiten (Entitäten)** identifizieren
* deren **Beziehungen** zueinander beschreiben
* diese passenden **CIDOC CRM-Klassen und -Eigenschaften zuordnen**
* Ergebnisaustausch im Plenum.


---

### Leitfragen

| Schritt | Leitfrage | Ziel |
|-------|-----------|------|
| 1 | Welche Kerneinheiten gibt es? | Kernentitäten identifizieren |
| 2 | Wie stehen die Kerneinheiten zueinander? | Beziehungen formulieren |
| 3 | Welche CIDOC CRM Klassen und Eigenschaften passen? | Semantische Modellskizze erstellen |

---

## Mini-Demo: CIDOC CRM in Kürze 

Wie werden grundlegende Klassen und Beziehungen in CIDOC CRM definiert? 

| CIDOC CRM Klasse | Bedeutung |
|------------------|-----------|
| **E28 Conceptual Object** | Spiel als geistiger Inhalt |
| **E22 Human-Made Object** | Physische Kopie (Cartridge, Disc, Box …) |
| **E21 Person** | Einzelne Mitwirkende |
| **E74 Group** | Studio, Entwicklerteam, Publisher |
| **E12 Production** | Herstellung / Veröffentlichung |
| **E42 Identifier** | Produktcodes, Inventarnummern, Seriennummern |

Quelle: [CIRCO CRM-Spezifikation (v7.1.3)](https://cidoc-crm.org/sites/default/files/cidoc_crm_version_7.1.3.pdf)  

---

## Ergebnis: Mindmap / Konzeptionelles Modell

![Konzept-Mindmap](../assets/Mindmap.png)

---

### Begründung der Modellierungsentscheidungen

| Pfad | Bedeutung | Warum so modelliert? |
|------|-----------|---------------------|
| **E73 → P102 has title → E35 Title** | Das Spiel hat einen Titel | Titel ist ein **eigenständiges Konzept**, nicht nur Text; ermöglicht Mehrsprachigkeit & Varianten |
| **E73 → P129 is about → E89 Propositional Object** | Das Spiel hat Eigenschaften | E89 erlaubt es, Merkmalsbündel strukturiert darzustellen und auf Quellen zurückzuführen |
| **E57 Type (Plattform) → P1 is identified by → E41 Appellation** | Plattform-Bezeichnung | Plattformen sind **kontrollierte Begriffe**, keine Freitexte |
| **E55 Type (Genre) → P1 is identified by → E41 Appellation** | Genre-Bezeichnung | Genre ist ein **Klassifikationsbegriff**; E55 unterstützt kontrollierte Vokabulare |
| **E99 Type (Edition) → P1 is identified by → E41 Appellation** | Edition / Version | Editionen sind **Domänenspezifika** → daher modelliert als Typen |

---

### Rolle von **E41 Appellation**

| Konzept | Erklärung |
|--------|-----------|
| **E41 Appellation** | Namen, Benennungen und Bezeichnungen sind **eigenständige Entitäten**, nicht nur Textstrings. Dies ermöglicht: Mehrsprachigkeit, Varianten, stabile IDs, Quellenangaben. |
| **P1 is identified by** | Verbindet das Konzept mit seiner **Benennung** → unterstützt Interoperabilität und Klarheit. |

---

## Datentyp-Eigenschaften in CIDOC CRM

CIDOC CRM …

* setzt Schwerpunkt auf **Beziehungen** zwischen Entitäten
* nutzt **Datentyp-Attribute nur sparsam**
* bevorzugt **semantische Identifikatoren** statt Freitext

Typische Datentyp-Eigenschaften (nur wenn nötig):

* verwendet Datentyp-Eigenschaften nur sparsam (z. B. P3 has note, P90 has value)
* legt den Schwerpunkt auf Beziehungen zwischen Entitäten
* nutzt Datentyp-Attribute ausschließlich für literale Werte.

Zentrale Informationen (Titel, Rollen, Identifikatoren, etc.) werden als eigene Entitäten modelliert und mit kontrollierten Vokabularen verknüpft.

Hinweis: Der Umgang mit Datentyp-Eigenschaften wird in den fortgeschrittenen Einheiten zu Vokabularen und Interoperabilität behandelt.

