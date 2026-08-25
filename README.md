# Terrain Drape GL

[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg?style=flat)](LICENSE.txt)

> [!IMPORTANT]
> This is an unofficial modified fork based on [MapLibre GL JS 6.2.0](https://github.com/maplibre/maplibre-gl-js).
> It is not affiliated with or endorsed by the MapLibre project or its contributors.
> MapLibre GL JS and MapLibre are names of their respective owners.

Terrain Drape GL preserves the MapLibre GL JS application API and adds terrain render-to-texture draping support for custom style layers.

## Fork changes

- Custom layers can opt into terrain draping with `terrainDrape` and `renderToTile`.
- Custom terrain textures are cached and invalidated through `terrainDrapeRevision`.
- Terrain rendering is selected by the renderer, so applications do not need to branch on terrain state.
- Custom terrain rendering is integrated into the existing terrain RTT layer stack.

## Installation

Install this fork under the `maplibre-gl` alias to keep existing application imports unchanged:

```sh
npm install maplibre-gl@npm:@hh-hang/maplibre-gl-custom-terrain-drape@6.2.0-terrain-drape.1
```

Then use the same imports as MapLibre GL JS:

```ts
import maplibregl from 'maplibre-gl';
import 'maplibre-gl/dist/maplibre-gl.css';
```

## Upstream project

This fork is derived from [MapLibre GL JS](https://github.com/maplibre/maplibre-gl-js). Refer to the upstream project for its general API documentation, examples, architecture, contribution history, and community information:

- [MapLibre GL JS documentation](https://maplibre.org/maplibre-gl-js/docs/API/)
- [MapLibre GL JS examples](https://maplibre.org/maplibre-gl-js/docs/examples/)
- [MapLibre GL JS source repository](https://github.com/maplibre/maplibre-gl-js)

Issues specific to this fork should be reported in the [fork repository](https://github.com/hh-hang/maplibre-gl-js/issues).

## License and attribution

This distribution retains the original copyright notices and is distributed under the [BSD-3-Clause license](LICENSE.txt).

The software includes work from MapLibre contributors, Mapbox GL JS 1.13 and earlier, and other authors identified in [LICENSE.txt](LICENSE.txt). The MapLibre and contributor names are used only to identify the origin of the software and do not imply endorsement of this fork.
