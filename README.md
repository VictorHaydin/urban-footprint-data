# urban-footprint-data

Map tiles for the [Urban Footprint](https://github.com/VictorHaydin/urban-footprint) web app
(«Структура міст»), published with GitHub Pages at <https://victorhaydin.github.io/urban-footprint-data/>.

Per city (`<city id>/`):

* `features.pmtiles` — vector tiles (z14) with every classified map feature;
* `overview.bin` — low-zoom raster pyramids (PMTiles, one per territory unit and category) packed into one
  file; their byte ranges are listed in the city's `stats.json` in the app repository.

The tiles are kept out of the app repository so that its GitHub Pages deploys stay small. They are generated
by the app's pipeline and copied here with `python -m urbanfp publish-tiles ../urban-footprint-data`.

Map data © OpenStreetMap contributors, available under the Open Database License (ODbL).
