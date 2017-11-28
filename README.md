
-----------------
# DEPRECATED
-----------------

## There is now an [ol package](https://www.npmjs.com/package/ol) that makes this `openlayers-prebuilt` package no longer necessary. Thanks OpenLayers team!



-----------------
-----------------


# Pre-built OpenLayers 3

This is simply a pre-built copy of the OpenLayers 3 JavaScript with no npm dependencies.

## Getting Started

- Install with npm: `npm install openlayers-prebuilt`


## Rationale

The only reason this package exists is to provide a smaller npm dependency list for those that don't need all the OpenLayers build tooling. This package will be obsolete if these issues are resolved:

- [https://github.com/openlayers/ol3/issues/3162](https://github.com/openlayers/ol3/issues/3162)
- [https://github.com/openlayers/ol3/issues/4141](https://github.com/openlayers/ol3/issues/4141)
- [https://github.com/openlayers/ol3/issues/4128](https://github.com/openlayers/ol3/issues/4128)

## Contributing

To update with a specific version of openlayers:
```
npm i openlayers@VERSION
rm -rf dist/
cp -r node_modules/openlayers/dist/ ./dist/
git commit -am "Updated to VERSION"
npm version VERSION
npm publish
```

