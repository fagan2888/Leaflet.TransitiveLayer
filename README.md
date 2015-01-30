
# Leaflet.TransitiveLayer

A [Leaflet](http://leafletjs.com/) plugin for overlaying a [Transitive.js](https://github.com/conveyal/transitive.js) map on a Leaflet map.

## Basic Usage

```
// create a Leaflet map (disabling inertia and zoom animation is recommended)
var map = L.map('map', {
  inertia: false,
  zoomAnimation: false
});

// create and add the base map layer
map.addLayer(new L.TileLayer(YOUR_TILE_URL));

// create the Transitive instance
var transitive = new Transitive({
  data: YOUR_TRANSITIVE_DATA
});

// create and add the Transitive layer to the map
map.addLayer(new L.TransitiveLayer(transitive));
```


## Running the Example

An example is provided with a sample Transitive data set.

In the example/ directory:
```
npm install
make
```
  
The first line installs [Component](https://github.com/componentjs/component); the second uses Component to download the Transitive.js dependency and build the example. Then open index.html in a web browser.



