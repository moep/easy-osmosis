Mapsforge - Easy Osmosis
========================
## About 
Easy Osmosis is a Ant build file for automatic installation of [Osmosis](http://wiki.openstreetmap.org/wiki/Osmosis) and the required plugins for creating map files to be used with the [Mapsforge](http://mapsforge.org) library.

## Installation
Map data can be downloaded from http://download.geofabrik.de/osm/.

1. `git clone git://github.com/moep/easy-osmosis.git`
2. `ant install`

## Map creation
Map files: `ant osm2map -Din=your_map.pbf.osm  -Dout=mapsforge_map.map`
POI DB: `ant osm2poi -Din=your_map.pbf.osm  -Dout=mapsforge_map.poi`

## Uninstall
Remove temporary files: `ant clean`
Remove installed files: `ant uninstall` (You have to delete ~/.openstreetmap/ manually afterwards.)



