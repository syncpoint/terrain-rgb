FROM osgeo/gdal:ubuntu-small-latest
# docker image containing all tools in order to transform a GeoTIFF into a PNG terrain tileset

LABEL MAINTAINER thomas.halwax@syncpoint.io

ENV LANG=C.UTF-8
ENV LC_ALL=C.UTF-8
## install pip3 and Mapbox's RasterIO (rio)
## install plugins for rio from https://github.com/mapbox/rasterio/wiki/Rio-plugin-registry
RUN apt-get -y update && apt-get install -y --fix-missing python3-pip vim proj-bin \
    && pip3 install rasterio \
    && pip3 install rio-rgbify \
    && pip3 install rio-mbtiles \
    && pip3 install mbutil \
    && apt-get clean
