# terrain-rgb
A detailed how-to to convert geo-tiff files containing DEM data into a pyramid of png files

## Motivation

Austria's gonvernment is fully commited to the idea of open data. A huge amount of data is published on [Austria's open data site](https://data.gv.at). This includes geo data like (vector) basemaps, contour lines, hillshading tiles and a lot more. Also Digital Elevation Model (DEM) data is available. The data is published as a huge (9 GB) GeoTIFF file. Although one may convert the file into a _Cloud Optimized GeoTIFF_ (COG), the goul of this how-to is to convert the GeoTIFF into a pyramid of PNG files that are contained in an MBTiles container.

Based on the model of [Mapbox Terrain-RGB](https://docs.mapbox.com/help/troubleshooting/access-elevation-data/) tileset we will document all steps required in order to create a similar set of tiles.

## Data

Since we mentioned Austria's Open Data initiative we will use the [DEM of Austria with a resolution of 10x10m](https://www.data.gv.at/katalog/dataset/b5de6975-417b-4320-afdb-eb2a9e2a1dbf).


