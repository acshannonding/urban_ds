# Types of Geospatial Data
https://pythongis.org/part2/chapter-05/nb/01-introduction-to-geographic-data-in-python.html

Vector

Raster

Spatio-Temporal

Topological

Vector
Ultimately rooted in Points, connected together in lines or polygons

Network
Vector-based consisting of nodes (points) and edges (lines)

Raster
Constructed from rectangular 'pixels' in a grid. Each cell contains metadata, e.g. elevation, temperature, or other attributes

good for zooming in and out, so particularly when you want multiple levels of view. Common for sattelite imagery

https://pythongis.org/_images/vector_vs_raster.jpg
points, lines and areas

point (tuple) -- can be 2 dimensional or 3 dimensional (e.g. x, y & sometimes z axis) coordinates are tuples

LineString (object) -- sequence of points joined in a line; at least 2 coord tuples

Polygon (obj) -- Filled Area with at least 3 coords, LinearRing is the linestring that encloses the area

MultiPoint, MultiLineString and MultiPolygon

https://pythongis.org/_images/vector_data_model.jpg

Types of files
Shapefile --- has 3 subfiles: '.shp' (feature geometries); '.shx' (positional index for geometries); .dbf (attribute info); Sometimes there's also a '.prj' with coord projection info

GeoJSON --- .geojson; simple text file

GeoPackage --- .gpkg

GML --- .gml (xml-based)

Coordinate reference systems ("CRS")

