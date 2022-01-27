# Mapping_Earthquakes
Mapping earthquake data and visualizing using javascript, D3, leaflet.js and Mapbox map API.

## Overview of the Analysis
Disaster Reporting Network is a non profit company that provides data driven storytelling on disasters around the world. As a data visualization specialist we have to build insightful data visualizations with interactive features on earthquakes around the world. By using, Leaflet.js and MAPBOX API to populate a geographical map with GeoJSON earthquake data from https://www.usgs.gov/programs/earthquake-hazards/earthquakes.

## Resources
* Software: HTML5, D3 js, Mapbox API , leaflet js
* GeoJSON Data: https://www.usgs.gov/programs/earthquake-hazards/

## Results
The html file can be found as [index.html]() and the javascript file for the challenge can be found in [challenge_logic.js]() and the css file an be found in [style.css]().

All the three layers and overlays are added as follows:
![layer_group_and_overlays](?raw=true)

The final result of all the three challenges is:
![default_page](?raw=true)

Here, you can see the base maps, street, satellite and dark in red which are radio buttons and only one option can be seen at one time. And the oveylay groups are checkboxes marked in green which can be seen together or in combination of one another.

#### Add Tectonic Plate Data:
![only_tectonic_plates](?raw=true)
* The tectonic plate data is added as a second layer group.
* The tectonic plate data is added to the overlay object.
* The d3.json() callback is working and does the following:
    1. The tectonic plate data is passed to the geoJSON() layer
    2. The geoJSON() layer adds color and width to the tectonic plate lines

![d1](?raw=true)
* The tectonic layer group variable is added to the map.

Finally, The earthquake data and tectonic plate data displayed on the map when the page loads.
![with_earthquake_techtonicplate](?raw=true)

#### Add Major Earthquake Data:
![only_major_earthquake](?raw=true)
The major earthquake data is added as a third layer group.
The major earthquake data is added to the overlay object.
The d3.json() callback is working and does the following: 
    1. Sets the color and diameter of each earthquake.
    2. The major earthquake data is passed to the geoJSON() layer.
    3. The geoJSON() layer creates a circle for each major earthquake, and adds a popup for each circle to display the magnitude and location of the earthquake
    4. The major earthquake layer group variable is added to the map

All the earthquake data and tectonic plate data are displayed on the map when the page loads and the datasets can be toggled on or off.
![satellite](?raw=true)

#### Add an Additional Map:
* Using the options from the Mapbox styles (Links to an external site.), add a third map style as a tile layer object to the challenge_logic.js file.
![third_layer](?raw=true)
* Added the map variable to the base layer object.
![third_base_layer](?raw=true)
* The index.html file where there are three map styles, and displays the two earthquake data sets and the tectonic plate data.
![dark](?raw=true)


