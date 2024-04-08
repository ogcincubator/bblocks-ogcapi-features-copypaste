
# Schema for extent (Schema)

`ogc.api.features.v1.schemas.extent` *v0.1*

This building block corresponds to the schema for an OGC API Records extent

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
allOf:
- $ref: https://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/extent.yaml
- properties:
    spatial:
      type: object
      properties:
        bbox:
          type: array
          items:
            ref: bblocks://ogc.geo.common.data_types.bounding_box

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/extent/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/extent/schema.yaml)

## Sources

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-features](https://github.com/ogcincubator/bblocks-ogcapi-features)
* Path: `_sources/v1/schemas/extent`

