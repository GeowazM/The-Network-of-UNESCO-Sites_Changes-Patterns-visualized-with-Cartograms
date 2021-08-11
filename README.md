

# <div align="center"> The Network of UNESCO Sites </div>
## <div align="center"> Changes and Patterns visualized with Cartograms </div>


### What we will learn
* How to plot data in QGIS
*	How to install a plugin
*	How to add further data
*	How to create a cartogram


### What we need
* Dataset "*UNESCO World Heritage in Danger*" (own research based on [UNESCO](https://whc.unesco.org/en/danger/), Copyright©1992-2021 UNESCO/World Heritage Centre. All rights reserved)</div>
* UN subregions scheme (Data source: [Countries](https://www.naturalearthdata.com/http//www.naturalearthdata.com/download/110m/cultural/ne_110m_admin_0_countries.zip), Scheme source: [UN subregion M49](https://unstats.un.org/unsd/methodology/m49/))
* Oceanic basemap (Source: [Natural Earth](https://www.naturalearthdata.com/))

> [**Download data here**](https://github.com/GeowazM/The-Network-of-UNESCO-Sites-Changes-and-Patterns-visualized-with-Cartograms/blob/main/data/Download-Data_UNESCO_World-Heritage_Sites-in-Danger_HIS-GIS.zip)


### What to do
1. Download the provided data & open in QGIS
2. Install plugins
3. Explore a World Heritage Site in Danger
4. Analyse the distribution of World Heritage Sites in Danger worldwide

<br/>

--- 

### The context we are working in
Since its foundation in 1945, the United Nations Educational, Scientific and Cultural Organization (UNESCO) became one of the most famous international institutions worldwide. With its different programs, the UNESCO has transformed itself into an important brand for the protection of cultural and natural landmarks. Continuously, the list of UNESCO designated sites is growing. However, the last five decades have been characterized by global economic and political changes, which have also repeatedly made it necessary for UNESCO to adapt. The List of World Heritage in Danger shows impressively, that also centuries-old properties have to accommodate to ascertained and potential sources of danger.<br/>
The constantly increase of UNESCO designated sites can be shown very well on the basis of tables and graphs. However, the regional weighting and influence of certain policies can barely be displayed with tables and numbers, if at all. Maps can be helpful, making the spatial distribution over varying times visible. By using cartograms, warping a regular map based on a certain value, the different weighting of the individual regions can be shown even more clearly. This allows an interpretation of past developments and implementation of the individual policies of UNESCO.
<br/>
<p align="center">
  <img src="/images/UNESCO_sites_overview.png" width="800" alt="Map of global distribution of UNESCO sites"/>
</p>

###### <div align="center"> Figure 1: Map of the global distribution of UNESCO Global Geoparks, Biosphere Reserves and World Heritage Sites within the UN subregions </div>

<br/>

---

## Hands-on<br/>

### Exercise 1
a) [Download](https://github.com/GeowazM/The-Network-of-UNESCO-Sites-Changes-and-Patterns-visualized-with-Cartograms/blob/main/data/Download_data_Network-of-UNESCO-Sites_HIS-GIS.zip) the data and open all files in QGIS. 
b) Take care about the project [coordinate reference system (CRS)](https://www.worldatlas.com/geography/world-map-robinson-projection.html). Set a equal-area projection, i.e. [World Robinson](http://epsg.io/54030) (EPSI: 54030). 
c) Your data should look like the map in figure 1. Have a look to the World Heritage Site "*Tasmanien Wilderness*". Have a look into the attribute table. 

#### I. When was the designation of the "*Tasmanian Wilderness*"?
#### II. How many hectares is covered by the "*Tasmanian Wilderness*"?


<br/>


### Exercise 2 
Now we are adding maps and satellite images to our project. Those can be used for orientation and simple analyses. This can be done by the large library of plugins which is offered by the [QGIS Plugin Repository](https://plugins.qgis.org/). 
a) The QGIS Plugin Manager enable us to install a Plugin directly in QGIS. [Watch this tutorial](https://www.youtube.com/watch?v=MVMzDY2RqQU&list=PL3NiwHdo_mtBDWWwYqAoDVs8JvsqAiRDp&index=1) (1 min) and install the *QuickMapServices (QMS)* plugin. 

<br/>


b) * Now add the [**OSM Standard**](https://www.openstreetmap.org/about) layer


To add satellite imagery via the "Bing Satellite Layer", we must extend the plugin by adding a contribution pack via <br>
>    *Web* <br>
>>   *QuickMapServices* <br>
>>>  *Settings* <br>
>>>>   *More services* <br>
>>>>>   *Get contributed pack* <br>

<br/>

c) * Now you can add the [**Bing Satellite**](https://www.arcgis.com/home/item.html?id=ae8ed793f2fb4ab0be1b7638082e95b5#:~:text=The%20Bing%20Maps%20aerial%20imagery,orthographic%20aerial%20and%20satellite%20imagery.&text=Bing%20Maps%20is%20continuously%20adding,not%20include%20bird's%20eye%20imagery) layer

<br/>


<p align="center">
  <img src="/images/whs_in_danger.PNG" width="800" alt="Map of the World Heritage in Danger (cartography: Mario Blersch, data: )"/>
</p>

###### <div align="center">  Figure 2: Example map with *Bing Satellite* as basemap </div>

<br/>


#### What's the difference of the **OSM Standard** and the **Bing Satellite** layer? 

<br/>

### Exercise 3
Explore the site [Abu Mena](http://whc.unesco.org/en/list/90/) in QGIS and online. 

#### I. Describe the land use around Abu Mena. 
#### II. Why is Abu Mena in danger? 
#### III. What is the advantage of a GIS?


<br/>

### Excersice 4
Now we need to know how many UNESCO sites in danger are within each UN subregion. 
a) Therefore, open the downloaded "*UN_subregions_with_UNESCO_sites.geojson*" file in QGIS. 
b) Check if every point is in a UN subregion. 
c) Then we add the number of UNESCO sites in danger (point features) to the UN subregions (polygon features) with the "*Count points in polygon*" algorithm. 

#### I. Open Processing Toolbox
>    *Processing* <br>
>>   *Toolbox* <br>
#### II. Search the "*Count points in polygon*" algorithm
#### III. Run the "*Count points in polygon*" algorithm
#### IV. Export the file as csv format
>    *Layer (right-click)* <br>
>>   *Export* <br>
>>>  *Save Features As...*  <br>

<br/>

Now you can use the csv file to create graphs i.e. in excel to support the visualization of a map.

<br/>

#### V. Which UN subregion show 15 World Heritage Sites in Danger?

<br/>

### Exercise 5
a) Follow the steps in Exercise 2 to install the [*cartogram3*](https://plugins.qgis.org/plugins/cartogram3/) plugin. 
b) Use the World Heritage in Danger file to calculate a cartogram. Generate a cartogram with the iterator 5, 10 and 15. 

#### I. What's the advantages and challenges of the iterator?​
#### II. Which continent show the most World Heritage in danger? 
#### III. What's the difference to the World Heritage cartogram below?

<br/>

<p align="center">
  <img src="/images/cartogram_World-Heritage-Sites_2011-2021_small.png" width="800" alt="Cartogram of the World Heritage Site designated sites between 2010 and 2021 (cartography: Mario Blersch, data: )"/>
</p>
  
###### <div align="center">  Figure 3: Cartogram of the World Heritage Site designated sites between 2010 and 2021 </div>




<br/>


---

<div align="center">
<img src="/images/rgeo_unesco-chair_uni-hd_v2.jpg" width="750" alt="rgeo Heidelberg University of Education"/>
</div>
