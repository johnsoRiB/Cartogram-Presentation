# Cartograms

> Spring 2017 | Geography 472/572 | Geovisualization: Geovisual Analytics
>
> By: Nick Mathews and Riley Johnson

## 1. What is a Cartogram?

A cartogram is a thematic map that displays a variable as a spacial dimension. Cartograms can represent socio-economic, population, or other types of variables by the distoring geometric space of a map. This distortion is intended to represent the variable data proportionally.

There are several types of cartograms that handle geometric distortion in a variety of ways. In general, some geometric quality of a cartogram will be preserved to achieve the desired aesthetic, such as: perimeter, neighborhood, or a combination of the two. 

## 2. Contiguous Cartograms

Contiguous cartograms preserve shape contact, or neighborhood, by simultaneiously skewing the shape geometry and size.

This example area cartogram shows the 2012 Presidential Election results. Each state is scaled relative to the number of electoral votes they have.
![cartogramUSelection_SongGao](img/cartogramUSelection_SongGao.jpg)
*Source: http://stko.geog.ucsb.edu/node/11*

This is a distance cartogram showing dynamic distance cartograms from any point, using any vehicle, mode, or time of year settings. For instance, the above cartogram from Carthago Nova. Cartograms can be run by clicking on sites or via a Cartogram tab that provides the same kind of interface as routes.
![o2cart](img/o2cart.png)
*Source: https://digitalhumanities.stanford.edu/projects/orbis*


## 3. Non-Contiguous Cartograms

Non-contiguous cartograms do not require shapes to preserve neighborhood. In other words, the shapes scale independently and no not touch either.

This cartogram, published by The New York Times, shows how much an individual's vote affects the electoral college, for each state. Note that a state's geometry is preserved as its size changes.
![non-contiguous-nytimes.png](img/non-contiguous-nytimes.png)
*Source: http://www.nytimes.com/interactive/2008/11/02/opinion/20081102_OPCHART.html*

### 3.1 Dorling Cartogram

This is an example of a Dorling cartogram. In this map, published by the Huffington post, states have been replaced with circles and scaled to represent electoral votes.
![dorling](img/dorling.png)
*Source: http://elections.huffingtonpost.com/2012/romney-vs-obama-electoral-map#cartogram*

## 4. Cartograms Using d3 & Topojson

The following code lists the data used to generate the cartogram. Birth rates, death rates, migration, etc. are all found within the data csv file.
http://prag.ma/code/d3-cartogram/#intlmig/2011

![d2carto](img/d2carto.JPG)

![d3examples](img/d3examples.JPG)

This d3 javascrpit library uses the Rubber Sheet Distortion method to create an area contiguous cartogram that preserves shape with distortion as well as preserving topology, although that is not guaranteed. 

The d3 library works by using a topojson to decocode topojson-encoded topologies. Takes topojson files converts them to another topojson that then is projected into the equal area map projection wit  the new distortion from the cartogram libraries algorithm.

This is the github repository where d3 cartogram can be downloaded from:
*Source: https://github.com/shawnbot/topogram*

## References:

[1] http://www.ncgia.ucsb.edu/projects/Cartogram_Central/types.html

[2] http://www.viz.tamu.edu/faculty/house/cartograms/Chapt-02.PDF
