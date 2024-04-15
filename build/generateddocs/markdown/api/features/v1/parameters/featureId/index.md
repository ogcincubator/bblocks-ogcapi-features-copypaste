
# Schema for limit (Parameter)

`ogc.api.features.v1.parameters.featureId` *v0.1*

This building block corresponds to the schema for an OGC API Records featureId

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
name: limit
in: query
description: 'The optional limit parameter limits the number of items that are presented
  in the response document.


  Only items are counted that are on the first level of the collection in the response
  document.

  Nested objects contained within the explicitly requested items shall not be counted.


  Minimum = 1. Maximum = 10000. Default = 10.'
required: false
schema:
  type: integer
  minimum: 1
  maximum: 10000
  default: 10
style: form
explode: false

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/featureId/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/featureId/schema.yaml)

## Sources

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-features](https://github.com/ogcincubator/bblocks-ogcapi-features)
* Path: `_sources/v1/parameters/featureId`

