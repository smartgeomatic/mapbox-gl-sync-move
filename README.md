# @mapbox/mapbox-gl-sync-move [![CircleCI](https://circleci.com/gh/mapbox/mapbox-gl-sync-move.svg?style=svg)](https://circleci.com/gh/mapbox/mapbox-gl-sync-move)

Sync movement between two or more [Mapbox GL JS](https://www.mapbox.com/mapbox-gl-js) maps.

## Install

```
npm install @mapbox/mapbox-gl-sync-move
```

## Usage

This module exports a function that receives as arguments two or more [Mapbox GL JS](https://www.mapbox.com/mapbox-gl-js) maps whose movements you'd like to sync.

```js
var mapboxgl = require('mapbox-gl');
var syncMove = require('mapbox-gl-sync-move');

var mapA = new mapboxgl.Map(..);
var mapB = new mapboxgl.Map(..);

var clearSync = syncMove(mapA, mapB);
clearSync()
```

## Developing

There are unit tests with mocked maps, and there's a page for manual testing.

Run the unit tests with `npm test`.

To manually test, ensure you have a `MapboxAccessToken` environment variable set. Then start the server with `npm run start`.
