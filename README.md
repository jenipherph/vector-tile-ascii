# vector-tile-ascii

ASCII renderer for OpenStreetMap vector tiles.

![Screenshot](examples/screenshot.png)


## Why?

Because it should be possible to download and view a single tile without configuring a massive Mapnik-based rendering infrastructure.


## Example

```bash
git clone https://github.com/vtduncan/vector-tile-ascii.git
cd vector-tile-ascii/

npm install

# Fetch and decompress a vector tile from MapBox
curl --compressed -o 10561.vector.pbf \
  "https://a.tiles.mapbox.com/v3/mapbox.mapbox-streets-v5/14/15881/10561.vector.pbf"

# View the tile
node index.js 10561.vector.pbf
```

Check it against the reference image:

![Map tile](examples/10561.png)

## Public domain

This is free software released into the public domain.
