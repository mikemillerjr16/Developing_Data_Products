---
title: "Data Products Week 2 Assignment"
author: "Mike Miller Jr."
date: "9/7/2019"
output:
  html_document:
    keep_md: yes
---



## Leaflet Map

Creating a Map that illustrates the Eiffel Tour


```r
library(leaflet)
```



```r
my_map <- leaflet() %>%
addTiles()
my_map
```

<!--html_preserve--><div id="htmlwidget-2a5ffbf667c1d885e158" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-2a5ffbf667c1d885e158">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]}]},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->



```r
EiffelTour <- c("<a href= 'http://www.toureiffel.paris' >Eiffel Tour</a>")
leaflet() %>%
addTiles() %>%
addMarkers(lat=48.858053, lng=2.294289, popup = EiffelTour)
```

<!--html_preserve--><div id="htmlwidget-4f04af89a7dd0148936e" style="width:672px;height:480px;" class="leaflet html-widget"></div>
<script type="application/json" data-for="htmlwidget-4f04af89a7dd0148936e">{"x":{"options":{"crs":{"crsClass":"L.CRS.EPSG3857","code":null,"proj4def":null,"projectedBounds":null,"options":{}}},"calls":[{"method":"addTiles","args":["//{s}.tile.openstreetmap.org/{z}/{x}/{y}.png",null,null,{"minZoom":0,"maxZoom":18,"tileSize":256,"subdomains":"abc","errorTileUrl":"","tms":false,"noWrap":false,"zoomOffset":0,"zoomReverse":false,"opacity":1,"zIndex":1,"detectRetina":false,"attribution":"&copy; <a href=\"http://openstreetmap.org\">OpenStreetMap<\/a> contributors, <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA<\/a>"}]},{"method":"addMarkers","args":[48.858053,2.294289,null,null,null,{"interactive":true,"draggable":false,"keyboard":true,"title":"","alt":"","zIndexOffset":0,"opacity":1,"riseOnHover":false,"riseOffset":250},"<a href= 'http://www.toureiffel.paris' >Eiffel Tour<\/a>",null,null,null,null,{"interactive":false,"permanent":false,"direction":"auto","opacity":1,"offset":[0,0],"textsize":"10px","textOnly":false,"className":"","sticky":true},null]}],"limits":{"lat":[48.858053,48.858053],"lng":[2.294289,2.294289]}},"evals":[],"jsHooks":[]}</script><!--/html_preserve-->

