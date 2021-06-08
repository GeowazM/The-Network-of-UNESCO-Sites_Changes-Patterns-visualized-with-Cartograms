# Abgabe 3 - Georeferenzieren und Digitalisieren

## Generelle Hinweise
* Team- oder Gruppenarbeit ist unzulässig und führt zum Nichtbestehen des Übungsblattes.
*	Die Abgabe erfolgt über die Lernplattform Moodle.
*	Es können maximal 100 Punkte erzielt werden.
*	Lest alle Hinweise, bevor ihr mit der Bearbeitung der Aufgaben beginnt.

## Zur Verfügung stehende Daten:
* TK50 L6316 Worms 2011 (Quelle: Hessisches Landesamt für Bodenmanagement nud Geoinformation 2011)
* Luftbild Fribourg (Quelle: [OpenAerialMap](https://map.openaerialmap.org), Provider: [Autonomous Imagery](https://www.autonomousimagery.com/))

Ladet euch [die Daten herunter](abgabe_03_data.zip) und speichert sie auf eurem PC. Legt einen lokalen Ordner (nicht auf einem Netzlaufwerk wie zum Beispiel "Q://Abgabe") an und speichert dort die obigen Daten. (.zip Ordner müssen vorher entpackt werden.)

## Abzugeben sind:
* Allgemein: Eine PDF-Datei „dokumentation“
* Aufgabe 1:
  * Die gesetzten Passpunkte als Tabelle
  * Ein Screenshot der Transformationseinstellungen
  * Ein Screenshot eurer georefenzierten Karte inklusive geeigneter Hintergrundlayer (z.B. OpenstreetMap)
  * eure georeferenzierte Karte müsst ihr **nicht** abgeben
* Aufgabe 2:
  * Die digitalisierten Layer, z.B. als Shapefiles
  * Ein Screenshot eures Ergebnisses mit angepasster Symbologie
* Führt diese Dateien in einen ZIP-Ordner zusammen, den ihr nach folgendem Muster benennt: Abgabe03_Vorname_Nachname (nutzt euren Vor- und Nachnamen). Ladet diesen final auf Moodle hoch.
* Hinweis 1: Abgaben ohne Dokumentation (als PDF) werden mit 0 Punkten bewertet!
* Hinweis 2: Unvollständige (und damit unlesbare) Shapefiles können nicht bewertet werden. Bei Shapefiles genügt es nicht die Datei mit der Endung `.shp` abzugeben. Auch die anderen Dateien mit den Endungen `.shx`, `.prj`, `.dbf`, `.cpg` (und falls vorhanden `.qpj`) müssen abgegeben werden.

Hinweise für die Dokumentation:
* gebt alle wesentlichen Schritte kurz und knapp an
* Stichpunkte genügen (bitte keine Romane! ;))
* Bitte gebt auf jeden Fall den Namen der Tools an, welche ihr genutzt habt
* falls ihr Parameter gewählt habt, nennt diese und liefert eine kurze Begründung, wenn der Parameterwert nicht eindeutig in der Aufgabenstellung gegeben war
* für Abgabe 03 sollte eure Dokumentation (ohne Screenshots) ungefähr 1-2 A4 Seite lang sein


## Aufgaben

### Aufgabe 1: Worms (50 Punkte)
* Georeferenziert die topographische Karte TK50 L6316 Worms 2011.
* Nutzt dafür **eine** der folgenden Methoden:
  * Georeferenzierung mit Kartenrandangaben in UTM
  * Georeferenzierung anhand eines Hintergrundlayers (z.B. OpenStreetMap-Webmap)
* Das Ergebnis sollte möglichst verzerrungsfrei sein. Nutzt daher geeignete Transformationseinstellungen
* Das Ziel besteht darin, einen RMS-Fehler von maximal 2 zu erreichen.


### Aufgabe 2: Freiburg im Üechtland, Schweiz (50 Punkte)
* Erstellt die folgenden Layer mithilfe des zur Verfügung stehenden Luftbilds:
  * Punkt-Layer (Kirchen, Parkplätze), insgesamt mind. 5 Features
  * Linien-Layer (Straßen, Brücken, Fluss), insgesamt mind. 15 Features
  * Polygon-Layer (Gebäude, Sportplätze), insgesamt mind. 15 Features
* achtet darauf die Sportplätze rechtwinklig zu kartieren
* Verseht die einzelnen Features jedes Layer mit Attributen, sodass man den Typ (beispielsweise "Kirche" oder "Parkplatz") unterscheiden kann
* passt das Styling der Daten so an, dass man die einzelnen Typen auch visuell einfach unterscheiden kann


**Viel Erfolg bei der Bearbeitung!**
