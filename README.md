# Mapping_Earthquakes
Mapping earthquake data and visualizing using javascript, D3, leaflet.js and Mapbox map API.

## Overview of the Analysis
Disaster Reporting Network is a non profit company that provides data driven storytelling on disasters around the world. As a data visualization specialist we have to build insightful data visualizations with interactive features on earthquakes around the world. By using, Leaflet.js and MAPBOX API to populate a geographical map with GeoJSON earthquake data from https://www.usgs.gov/programs/earthquake-hazards/earthquakes.

## Resources
* Software: HTML5, D3 js, Mapbox API , leaflet js
* GeoJSON Data: https://www.usgs.gov/programs/earthquake-hazards/

## Results
The html file can be found as [index.html](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/index.html) and the javascript file for the challenge can be found in [challenge_logic.js](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/js/challenge_logic.js) and the css file can be found in [style.css](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/css/style.css).

All the three layers and overlays are added as follows:
![layer_group_and_overlays](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/layer_group_and_overlays.png?raw=true)

The final result of all the three challenges is:
![default_page](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/default_page.png?raw=true)

Here, you can see the base maps, street, satellite and dark in red which are radio buttons and only one option can be seen at one time. And the oveylay groups are checkboxes marked in green which can be seen together or in combination of one another.

### Tectonic Plate Data:
![only_tectonic_plates](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/only_tectonic_plates.png?raw=true)
* The tectonic plate data is added as a second layer group.
* The tectonic plate data is added to the overlay object.
* The d3.json() callback is working and does the following:
    1. The tectonic plate data is passed to the geoJSON() layer
    2. The geoJSON() layer adds color and width to the tectonic plate lines

![d1](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/d1.png?raw=true)
* The tectonic layer group variable is added to the map.

Finally, The earthquake data and tectonic plate data displayed on the map when the page loads.
![with_earthquake_techtonicplate](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/with_earthquake_techtonicplate.png?raw=true)

### Major Earthquake Data:
![only_major_earthquake](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/only_major_earthquake.png?raw=true)
The major earthquake data is added as a third layer group.
The major earthquake data is added to the overlay object.
The d3.json() callback is working and does the following: 
    1. Sets the color and diameter of each earthquake.
    2. The major earthquake data is passed to the geoJSON() layer.
    3. The geoJSON() layer creates a circle for each major earthquake, and adds a popup for each circle to display the magnitude and location of the earthquake
    4. The major earthquake layer group variable is added to the map

All the earthquake data and tectonic plate data are displayed on the map when the page loads and the datasets can be toggled on or off. In a satellite view
![satellite](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/satellite.png?raw=true)

### Additional Map:
* Using the options from the Mapbox styles (Links to an external site.), add a third map style as a tile layer object to the challenge_logic.js file.
![third_layer](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/third_layer.png?raw=true)
* Added the map variable to the base layer object.

![third_base_layer](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/third_base_layer.png?raw=true)
* The index.html file where there are three map styles, and displays the two earthquake data sets and the tectonic plate data.
![dark](https://github.com/sucharita1/Mapping_Earthquakes/blob/fec16154e7dc0c47b92a7ff558d78cc29c0dd968/Earthquake_Challenge/static/images/dark.png?raw=true)


