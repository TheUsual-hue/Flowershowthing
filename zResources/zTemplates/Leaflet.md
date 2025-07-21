---
map_height_y: 2048
map_width_x: 1642
scale_pixels: 268
scale_pixels_range: 25
mapCalc1: 0.09328358208955223
---

> [!NOTE]- Quick Calculator  
> Map Height in Pixels: `INPUT[number:map_height_y]`  
> Map Width in Pixels: `INPUT[number:map_width_x]`  
> lat: `VIEW[{map_height_y} / 2][math]`  
> long: `VIEW[{map_width_x} / 2][math]`  
> How Many Pixels In Scale: `INPUT[number:scale_pixels]`  
> How Many Units in Scale: `INPUT[number:scale_pixels_range]`  
> Scale: `VIEW[1/({scale_pixels}/{scale_pixels_range})][math:mapCalc1]`



```leaflet  
id: MapCalcExample  
image:  
bounds: [[0,0], [2048, 1642]] 
height: 850px   
width: 95%  
lat: 1024  
long: 821   
minZoom: -1.5  
maxZoom: 1  
defaultZoom: -1 
zoomDelta: 0.5   
unit: mi   
scale: 0.09328358208955223   
recenter: false  
darkmode: false 
```
