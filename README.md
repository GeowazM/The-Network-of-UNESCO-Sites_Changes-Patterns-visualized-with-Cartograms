# The Network of UNESCO Sites - Changes and Patterns visualized with Cartograms

## Tasks
* Plot the "*World Heritage in Danger*" data set
*	Install plugins in QGIS
*	Add a WMTS layer
*	Create a cartogram


## Data:
* UNESCO List of "*World Heritage in Danger*" (Source: [UNESCO](https://whc.unesco.org/en/danger/), Copyright©1992-2021 UNESCO/World Heritage Centre. All rights reserved)
* UN subregions scheme (Source: [UN subregion M49](https://unstats.un.org/unsd/methodology/m49/), [Wiki](https://en.wikipedia.org/wiki/United_Nations_geoscheme))
* Land basemap (Source: [Natural Earth](https://www.naturalearthdata.com/http//www.naturalearthdata.com/download/110m/physical/ne_110m_land.zip))
* Ocean basemap (Source: [Natural Earth](https://www.naturalearthdata.com/http//www.naturalearthdata.com/download/110m/physical/ne_110m_ocean.zip))


## Context
Since its foundation in 1945, the United Nations Educational, Scientific and Cultural Organization (UNESCO) became one of the most famous international institutions worldwide. With its different programs, the UNESCO has transformed itself into an important brand for the protection of cultural and natural landmarks. Continuously, the list of UNESCO designated sites is growing. However, the last five decades have been characterized by global economic and political changes, which have also repeatedly made it necessary for UNESCO to adapt. The List of World Heritage in Danger shows impressively, that also centuries-old properties have to accommodate to ascertained and potential sources of danger. As the political and economic importance of UNESCO has increased, so has the media attention about the UNESCO and its decisions. It is a balancing act to make sensible decisions as a global institution that affect the lives of individuals in different regions around the world.
The constantly increase of UNESCO designated sites can be shown very well on the basis of tables and graphs. However, the regional weighting and influence of certain policies can barely be displayed with tables and numbers, if at all. Maps can be helpful, making the spatial distribution over varying times visible. By using cartograms, warping a regular map based on a certain value, the different weighting of the individual regions can be shown even more clearly. This allows an interpretation of past developments and implementation of the individual policies of UNESCO.

### Map
<p align="center">
  <img src="/images/UNESCO_sites_overview.png" width="800" alt="Sublime's custom image"/>
</p>
Map of the global distribution of UNESCO Global Geoparks, Biosphere Reserves and World Heritage Sites within the UN subregions.


## Excersice

### Aufgabe 1 (15 Punkte)
Extrahiert das Gebiet der Dammer Oberkreidemulde inklusive der umliegenden Höhenzüge (Gehn, Stemweder Berg, Dammer Berge, direkt südlich angrenzender Teil des Wiehengebirges) aus dem Gesamtdatensatz (TANDEM-X-Höhenraster). Erstellt dabei einen rechteckigen Ausschnitt. Stellt sicher, dass die Daten in einer geeigneten Projektion vorliegen (UTM 32N).

### Aufgabe 2 (35 Punkte)
Berechnet die lokalen Geländekrümmungen (Curvature) für den in Aufgabe 1 extrahierten Ausschnitt. Ermittelt hierbei zwei Arten der Geländekrümmung (siehe untenstehende Abbildung):

* a) Profilkrümmung (englisch: profile),
* b) Horizontalkrümmung (englisch: planform/plan).

Eine positive Profilkrümmung gibt eine konkave Krümmung an, was die Fließgeschwindigkeit von abfließendem Wasser erhöht. Bei der horizontalen Krümmung sind hingegen negative Werte von größerer Bedeutung für die Erosion, da dies Wasserflüsse bündelt und so die Fließgeschwindigkeit und den Bodenabtrag noch stärker beschleunigt.


### Aufgabe 3 (15 Punkte)
Berechnet die Geländeneigung (Slope) in Grad für das extrahierte Gebiet. Speichert diese ebenfalls in ein GeoTIFF.

### Aufgabe 4 (35 Punkte)
Ermittelt zunächst die Flächen:
* (i) in denen einerseits die Geländeneigung mindestens 7° beträgt
* (ii) in denen die Profilkrümmung größer als 0.001,
* (iii) in denen die Horizontalkrümmung kleiner als -0.001.

Erstellt darauf basierend ein Raster, in dem die Werte die Anzahl der vorhandenen obigen Risikofaktoren (i) bis (iii) widerspiegeln (d.h., wenn alle Faktoren vorliegen, soll das Raster den Wert 3 annehmen etc.). Speichert auch dieses Raster in einem GeoTIFF.

**Viel Erfolg bei der Bearbeitung!**
