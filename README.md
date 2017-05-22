# Cartogram

> Spring 2017 | Geography 472/572 | Geovisualization: Geovisual Analytics
>
> By: Nicholas Matthews and Riley Johnson

## 1. What is a Cartogram

A cartogram is thematic map that displays a variable as a size or distance. These variables can be things like socio-economic factors, population, or other. Then geometric space of the map is then distorted to display the data proportionally.

![cartogramUSelection_SongGao](C:\Oregon State\OSU 2016-2017\Spring Term 2017\GEOG 472\cartogram\img\cartogramUSelection_SongGao.jpg)

*Source: http://stko.geog.ucsb.edu/node/11*

This is an example area cartogram showing the 2012 Presidential Election results. Each state is scaled relative to the number of electoral votes they have. 

![o2cart](C:\Oregon State\OSU 2016-2017\Spring Term 2017\GEOG 472\cartogram\img\o2cart.png)

*Source: https://digitalhumanities.stanford.edu/projects/orbis*

This is a distance cartogram showing dynamic distance cartograms from any point, using any vehicle, mode, or time of year settings. For instance, the above cartogram from Carthago Nova. Cartograms can be run by clicking on sites or via a Cartogram tab that provides the same kind of interface as routes.





## 2. Cartograms using d3 & Topojson

http://prag.ma/code/d3-cartogram/#intlmig/2011

![d2carto](C:\Oregon State\OSU 2016-2017\Spring Term 2017\GEOG 472\cartogram\img\d2carto.JPG)

![d3examples](C:\Oregon State\OSU 2016-2017\Spring Term 2017\GEOG 472\cartogram\img\d3examples.JPG)



This d3 javascrpit library uses the Rubber Sheet Distortion method to create an area contiguous cartogram that preserves shape with distortion as well as preserving topology, although that is not guaranteed. 



The d3 library works by using a topojson to decocode topojson-encoded topologies. Takes topojson files converts them to another topojson that then is projected into the equal area map projection wit  the new distortion from the cartogram libraries algorithm.



*Source: https://github.com/shawnbot/topogram*

This is the github repository where d3 cartogram can be downloaded from.