# USA Airport Map

Choropleth Map of Airports in the United States.

## Introduction

This visualization shows where airports are located in every US State.
Red plane icons signify airports with a control tower. Grey plane icons
signify airports without control towers. States are colored according
to the number of airports they have. For example, Alaska has the most airports
in the USA, so it is the darkest shade. South Dakota has relatively few airports so it is the lightest shade. Interestingly, most of Alaska's airports do not have control towers. These are likely small, remote landing strips. If we ignore airports without control towers, then California, Texas, and Florida will be the top states.

## Primary Functions

The program loads airport geodata from geojson files and places location markers on the map. When an airport marker is clicked, the marker bounces and shows a popup with
the airport's name. The program also visualizes the number of airports per state as a Choropleth map.

*setColor(density)
  -\@param density : state airport count
  -bins states based on their number of airports
  -assigns colors to bins
*style(feature)
  -\@param feature : state polygon feature
  -appropriately styles each state to create Choropleth Map


## Libraries

This visualization primarily makes use of the Leaflet library.
I used a Leaflet plugin called SmoothMarkerBouncing to implement a bounce action
when a marker is clicked.
Icons from Font Awesome library.
Icon color from Chroma.js.
Map colors from ColorBrewer.

## Data Sources/Acknowledgments

This lab comes from Professor Bo Zhao at the University of Washington.
Airport data courtesy of USGS.
State Boundary data courtesy of Mike Bostock, D3js.
