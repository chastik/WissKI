<!--

icon: https://raw.githubusercontent.com/chastik/Beratung_Dateityp_Bild/refs/heads/main/SODa-Logo_full.svg
link: https://raw.githubusercontent.com/chastik/Beratung/refs/heads/main/soda.css

-->

# SODa WissKI Bits 

**Modul 2 DATENMODELL ENTWICKELN UND IMPLEMENTIEREN AM BEISPIEL** 

Vom Diagramm zu Pfaden – Erläutern und anwenden

Einheit 3: **WissKI Pathbuilder-Datei erzeugen**

Duration: ~ 25 Min.

---

## Von Ontologiebeziehungen zu WissKI-Pfaden

Da WissKI kann Ontologiedateien nicht direkt interpretieren und benötigt explizite **semantische Pfade**, um:

* den RDF-Wissensgraphen aufzubauen und  
* eine ontologiekonforme Datenspeicherung zu gewährleisten
* und Dateneingabeformulare zu strukturieren und zu organisieren.  

Die Ontologiemodellierung konzentriert sich auf die Beschreibung von **Klassen** und **semantischen Beziehungen**.  

WissKI implementiert diese Verbindungen als **Pfade** – also Sequenzen von Ontologie-Properties.

Jede semantische Sequenz wird im WissKI Pathbuilder zu **einem Pfad**.

---

### Beispiel

**Ontologiebeziehung**

Computer Game → wurde erstellt in → Creation Event → durchgeführt von → Group

**WissKI-Gruppe und Pfade**

Computer Game (Group)

* → **P94 wurde erstellt durch** → Creation Event  (Pfad)  
* → **P14 durchgeführt von** → Group  (Pfad)

**Hinweis:** Wenn **E12 Production Event** anstelle von **E65 Creation Event** verwendet werden würde, entstünde ein semantischer Fehler, da **E12 Production Event** nicht mit **P94 wurde erstellt durch** kompatibel ist.  

Genau hier ist eine semantische Validierung wertvoll und liefert aussagekräftige Rückmeldungen.

---

## Was ist der Pathbuilder?

Der **Pathbuilder** ist die Implementierungsschicht von WissKI. Anstelle relationaler Tabellen verwendet er **semantische Pfade**.  

Pfade definieren die interne Ontologiestruktur von WissKI und werden genutzt, um Dateneingabeformulare und RDF-Tripel zu generieren — diese Aspekte werden in einer späteren Einheit vertieft.

<table>
  <tr>
    <td><img src="../assets/WissKI_pathbuilder.jpg" alt="WissKI Pathbuilder" width="75%"></td>
  </tr>
</table>

---

## Workflow

| Schritt | Aktion                                |
| -------- | ------------------------------------ |
| 1        | draw.io-Modell als .xml exportieren  |
| 2        | In den WissKI Pathbuilder-Web Service hochladen |
| 3        | Pipeline validiert die Ontologiestruktur |
| 4        | **WissKI Pathbuilder XML** generieren |
| 5        | XML in WissKI importieren    |
| 6        | Pfade erscheinen automatisch |
| 7        | Pfadstruktur prüfen |


Dieser Prozess überbrückt die Lücke zwischen der Ontologiemodellierung und der internen Datenstruktur von WissKI, indem das semantische draw.io-Modell über eine Transformationspipeline automatisch in WissKI-Pfade umgewandelt wird.

---

## Praktische Aufgabe (Partnerarbeit – 20 Min.)

| Nr. | Schrittbeschreibung | Grafik |
| --- | ------------------- | ------- |
| 1 | Export des Draw.io-Modells ([Beispiel-Draw.io-Diagramm](https://drive.google.com/file/d/1CzgpEMxGYmfUgI2LUh0J-cbfsfW82T3f/view?usp=sharing)) als .xml-Datei ([Beispiel-Draw.io-XML-Datei](https://isl.ics.forth.gr/gnm_services/files/examples/diagrams_to_pathbuilders/DrawioPathBuilderExampleInput.xml)) | ![Platzhalter](../assets/schritt1.png) |
| 2 | Hochladen in [Draw.io-Diagramme-zu-WissKI-Pathbuilder-Webdienst](https://isl.ics.forth.gr/gnm_services/drawioXMLtoWisskiPathbuilder/) | ![Platzhalter](../assets/schritt2.png) |
| 3 | Pathbuilder-XML-Datei generieren und Link-Adresse kopieren ([Beispiel-Pathbuilder-XML-Datei](https://isl.ics.forth.gr/gnm_services/files/examples/diagrams_to_pathbuilders/DrawioPathBuilderExampleOutput.xml)) | ![Platzhalter](../assets/schritt3.png) |
| 4 | In WissKI einloggen | ![Platzhalter](../assets/schritt4.png) |
| 5 | Prüfen, ob in WissKI bereits CIDOC CRM geladen ist, siehe „Configuration/Ontology/Default WissKI Distillery Adapter“ | ![Platzhalter](../assets/schritt5.png) |
| 6 | Zu „Configuration/Pathbuilder“ navigieren | ![Platzhalter](../assets/schritt6.png) |
| 7 | Neuen Pathbuilder hinzufügen „Add Pathbuilder“, Name vergeben und speichern | ![Platzhalter](../assets/schritt7.png) |
| 8 | Unter „Pathbuilder Definition Import“ zuvor kopierte Link-Adresse einfügen und „Import“ klicken | ![Platzhalter](../assets/schritt8.png) |
| 9 | Die erzeugten semantischen Pfade prüfen | ![Platzhalter](../assets/schritt9.png) |
|10| Ergebnis: WissKI Pathbuilder auf Basis des eigenen Domänenmodells||

---

## Vorteile der draw.io → Pathbuilder-XML-Pipeline

Diese Pipeline wandelt draw.io-Ontologiediagramme automatisch in WissKI-Pathbuilder-XML-Dateien um und bietet mehrere Vorteile:

* **Zeiteffizienz** – beseitigt den manuellen Konvertierungsaufwand  
* **Ontologie-Wiederverwendung** – nutzt vorhandene Ontologielogik  
* **Konsistenz** – gewährleistet eine einheitliche Struktur über Dateien hinweg  
* **Semantische Integrität** – bewahrt die ursprüngliche Bedeutung und Beziehungen  

---

## Hintergrund: Wie die Pipeline funktioniert

Der [FORTH-ICS-Webdienst](https://isl.ics.forth.gr/gnm_services/):

* analysiert draw.io-Diagramme über eine **JSON-Konfiguration**  
* erkennt **semantische Pfade** von einem **zentralen Ontologieknoten** aus  
* überprüft die **syntaktische Gültigkeit** anhand der Ontologiedateien  
* exportiert die Pfade als **WissKI Pathbuilder XML**

---






