---
title: Schema for extent (Schema)

toc_footers:
  - Version 0.1
  - <a href='#'>Schema for extent</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: Schema for extent (Schema)
---


# Schema for extent `ogc.api.features.v1.schemas.extent`

This building block corresponds to the schema for an OGC API Features extent

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong>valid</strong>
</aside>


# JSON Schema

```yaml--schema
$comment: Adapted from https://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/extent.yaml
description: 'The extent of the features in the collection. In the Core only spatial
  and temporal

  extents are specified. Extensions may add additional members to represent other

  extents, for example, thermal or pressure ranges.


  An array of extents is provided for each extent type (spatial, temporal). The first
  item

  in the array describes the overall extent of the data. All subsequent items describe
  more

  precise extents, e.g., to identify clusters of data. Clients only interested in
  the

  overall extent will only need to access the first extent in the array.'
type: object
properties:
  spatial:
    description: The spatial extent of the features in the collection.
    type: object
    properties:
      bbox:
        type: array
        items:
          ref: bblocks://ogc.geo.common.data_types.bounding_box
      crs:
        description: 'Coordinate reference system of the coordinates in the spatial
          extent

          (property `bbox`). The default reference system is WGS 84 longitude/latitude.

          In the Core the only other supported coordinate reference system is

          WGS 84 longitude/latitude/ellipsoidal height for coordinates with height.

          Extensions may support additional coordinate reference systems and add

          additional enum values.'
        type: string
        enum:
        - http://www.opengis.net/def/crs/OGC/1.3/CRS84
        - http://www.opengis.net/def/crs/OGC/0/CRS84h
        default: http://www.opengis.net/def/crs/OGC/1.3/CRS84
  temporal:
    description: The temporal extent of the features in the collection.
    type: object
    properties:
      interval:
        description: 'One or more time intervals that describe the temporal extent
          of the dataset.

          In the Core only a single time interval is supported.


          Extensions may support multiple intervals.

          The first time interval describes the overall

          temporal extent of the data. All subsequent time intervals describe

          more precise time intervals, e.g., to identify clusters of data.

          Clients only interested in the overall temporal extent will only need

          to access the first time interval in the array (a pair of lower and upper

          bound instants).'
        type: array
        minItems: 1
        items:
          description: 'Begin and end times of the time interval. The timestamps are
            in the

            temporal coordinate reference system specified in `trs`. By default

            this is the Gregorian calendar.


            The value `null` at start or end is supported and indicates a half-bounded
            interval.'
          type: array
          minItems: 2
          maxItems: 2
          items:
            type: string
            format: date-time
            nullable: true
          example:
          - '2011-11-11T12:22:11Z'
          - null
      trs:
        description: 'Coordinate reference system of the coordinates in the temporal
          extent

          (property `interval`). The default reference system is the Gregorian calendar.

          In the Core this is the only supported temporal coordinate reference system.

          Extensions may support additional temporal coordinate reference systems
          and add

          additional enum values.'
        type: string
        enum:
        - http://www.opengis.net/def/uom/ISO-8601/0/Gregorian
        default: http://www.opengis.net/def/uom/ISO-8601/0/Gregorian

```

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Fannotated%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fextent%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/extent/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/extent/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/extent/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/extent/schema.json</a>

# References

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-ogcapi-features" target="_blank">https://github.com/ogcincubator/bblocks-ogcapi-features</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-ogcapi-features/blob/HEAD/_sources/v1/schemas/extent" target="_blank">_sources/v1/schemas/extent</a></code>

