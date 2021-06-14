# The Network of UNESCO Sites -
# Changes and Patterns visualized with Cartograms

## Tasks
* Plot the "*World Heritage in Danger*" data set
*	Install plugins in QGIS
*	Add a WMTS layer
*	Create a cartogram


## Data:
* UNESCO List of "*World Heritage in Danger*" (Source: [UNESCO](https://whc.unesco.org/en/danger/), Copyright©1992-2021 UNESCO/World Heritage Centre. All rights reserved)
* UN subregions scheme (Data source: [Countries](https://www.naturalearthdata.com/http//www.naturalearthdata.com/download/110m/cultural/ne_110m_admin_0_countries.zip), Scheme source: [UN subregion M49](https://unstats.un.org/unsd/methodology/m49/))
* Oceanic basemap (Source: [Natural Earth](https://www.naturalearthdata.com/))

[**Download data**](https://github.com/GeowazM/The-Network-of-UNESCO-Sites-Changes-and-Patterns-visualized-with-Cartograms/blob/main/data/Download_data_Network-of-UNESCO-Sites_HIS-GIS.zip)

<br/>
<br/>

## Table of content:
1. [Download data](https://github.com/GeowazM/The-Network-of-UNESCO-Sites-Changes-and-Patterns-visualized-with-Cartograms/blob/main/data/Download_data_Network-of-UNESCO-Sites_HIS-GIS.zip), unzip & open in QGIS
2. Install plugins
3. Explore the World Heritage Site [Abu Mena](http://whc.unesco.org/en/list/90/)
4. Analyse the distribution of World Heritage in Danger worldwide

<br/>

## Context
Since its foundation in 1945, the United Nations Educational, Scientific and Cultural Organization (UNESCO) became one of the most famous international institutions worldwide. With its different programs, the UNESCO has transformed itself into an important brand for the protection of cultural and natural landmarks. Continuously, the list of UNESCO designated sites is growing. However, the last five decades have been characterized by global economic and political changes, which have also repeatedly made it necessary for UNESCO to adapt. The List of World Heritage in Danger shows impressively, that also centuries-old properties have to accommodate to ascertained and potential sources of danger. As the political and economic importance of UNESCO has increased, so has the media attention about the UNESCO and its decisions. It is a balancing act to make sensible decisions as a global institution that affect the lives of individuals in different regions around the world.
The constantly increase of UNESCO designated sites can be shown very well on the basis of tables and graphs. However, the regional weighting and influence of certain policies can barely be displayed with tables and numbers, if at all. Maps can be helpful, making the spatial distribution over varying times visible. By using cartograms, warping a regular map based on a certain value, the different weighting of the individual regions can be shown even more clearly. This allows an interpretation of past developments and implementation of the individual policies of UNESCO.
<br/>
<p align="center">
  <img src="/images/UNESCO_sites_overview.png" width="800" alt="Map of global distribution of UNESCO sites"/>
</p>
Figure 1: Map of the global distribution of UNESCO Global Geoparks, Biosphere Reserves and World Heritage Sites within the UN subregions.

<br/>
<br/>
<br/>

## Excersice

### Excersice 1
[Download](https://github.com/GeowazM/The-Network-of-UNESCO-Sites-Changes-and-Patterns-visualized-with-Cartograms/blob/main/data/Download_data_Network-of-UNESCO-Sites_HIS-GIS.zip) the data and open all data files in QGIS. Take care about the project coordinate reference system (CRS). Set a equal-area projection, i.e. [World Robinson](http://epsg.io/54030). Your data should look like the map in figure 1.
<br/>


### Excersice 2 
Now we are adding more opportunities to our project. This can be done by the large library of plugins which is offered by the [QGIS Plugin Repository](https://plugins.qgis.org/). The QGIS Plugin Manager enable us to install a Plugin directly in QGIS. [Watch this tutorial](https://www.youtube.com/watch?v=Qf0MPTzf6Ow) (1 min) and install the *QuickMapServices* (QMS) plugin. 
<br/>


* Now add the [**OSM Standard**](https://www.openstreetmap.org/about) layer


After the installatation you can extend the plugin by adding a contrbution pack via 
I.   *Web* 
II.  *QuickMapServices* 
III. *Settings*
IV.  *More services*
V.   *Get contributed pack*
<br/>


* Add the [**Bing Satellite**](https://www.arcgis.com/home/item.html?id=ae8ed793f2fb4ab0be1b7638082e95b5#:~:text=The%20Bing%20Maps%20aerial%20imagery,orthographic%20aerial%20and%20satellite%20imagery.&text=Bing%20Maps%20is%20continuously%20adding,not%20include%20bird's%20eye%20imagery) layer


Your data should somewhow look like the image below:
<p align="center">
  <img src="/images/world_heritage_test.png" width="800" alt="Map of the World Heritage in Danger"/>
</p>

### Excersice 3
Explore the site [Abu Mena](http://whc.unesco.org/en/list/90/). Do you know why this World Heritage Site is in danger? Whats the advantage of the GIS?

*Solution: [Indicators](http://whc.unesco.org/en/list/90/indicators/)*
<br/>




### Aufgabe 4 (35 Punkte)
Follow the steps in excersice 2 to install the [*cartogram3*](https://plugins.qgis.org/plugins/cartogram3/) plugin. Use the World Heritage in Danger file to calculate a cartoram.



