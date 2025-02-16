# leaflet-challenge
The code for the map displayed when clicking on the index.html file within the "Leaflet-Part-1" folder in the leaflet-challenge repository can be found in the logic.js file (Leaflet-Part-1 --> static --> js --> logic.js).

All of the code was written completely independently with the help of the Xpert AI tool.

First and foremost, a base map was created to set the background using L.tilelayer and the open street map API. Then, a zoom and center feature were added to make the map more structured and interactive. Finally, layer groups representing our earthquake and tectonic plate data were added to give us the desired visualizations using L.layerGroup().

d3.json was used to make a request to get the earthquake data that we are attempting to display on the map. Next, function styleInfo (feature) was used to add all of the details on each earthquake represented on the map like depth and magnitude. In order to create a visually pleasant map that is easy to follow, the depth numbers were used to represent the earthquakes differently by color using function getColor (depth). Finally, function getRadius (magnitude) was used to add this additional information from the magnitude data.

Finally, L.GeoJson is used to add stylistic features to the map such as rendering each feature into a circleMarker that can be modified based on the differences in the earthquakes magnitudes and depths. The code .addTo(myMap) was used to add both the earthquake layer and the legend to the final map which displays as expected on any browser. I chose to display it on Google Chrome for verification. 