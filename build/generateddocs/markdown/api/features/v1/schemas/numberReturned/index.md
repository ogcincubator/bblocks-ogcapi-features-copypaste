
# Schema for numberReturned (Datatype)

`ogc.api.features.v1.schemas.numberReturned` *v0.1*

This building block corresponds to the schema for an OGC API Records numberReturned

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
description: 'The number of features in the feature collection.


  A server may omit this information in a response, if the information

  about the number of features is not known or difficult to compute.


  If the value is provided, the value shall be identical to the number

  of items in the "features" array.'
type: integer
minimum: 0
example: 10

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/numberReturned/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/numberReturned/schema.yaml)

## Sources

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-features](https://github.com/ogcincubator/bblocks-ogcapi-features)
* Path: `_sources/v1/schemas/numberReturned`

