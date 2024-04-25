
# Schema for collection (Schema)

`ogc.api.features.v1.schemas.collection` *v0.1*

This building block corresponds to the schema for an OGC API Features collection

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Road collection
#### json
```json
{
   "id": "roadl_1m",
   "title": "Roads",
   "extent":
   {
      "spatial":  {
         "bbox": [
            [-179.999420166016,-54.88802337646479,
              179.9999,74.740592956543]
         ],
         "crs": "http://www.opengis.net/def/crs/OGC/1.3/CRS84"
      },
      "temporal": {
         "interval": [
            ["2017-01-01T00:00:00Z","2017-12-31T23:59:59Z"]
         ],
         "trs": "http://www.opengis.net/def/uom/ISO-8601/0/Gregorian"
      }
   },
   "links": [
      {
        "rel": "self",
        "title": "This document",
        "type": "application/json",
        "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=application%2Fjson"
      },
      {
        "rel": "alternate",
        "title": "This document as HTML",
        "type": "text/html",
        "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=text%2Fhtml"
      },
      {
         "rel": "items",
         "title": "Roads",
         "type": "application/geo+json",
         "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=application%2Fgeo%2Bjson"
      },
      {
         "rel": "items",
         "title": "Roads",
         "type": "text/html",
         "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=text%2Fhtml"
      },
      {
         "rel": "items",
         "title": "Roads",
         "type": "application/gml+xml;version=3.2;profile=\"http://www.opengis.net/def/profile/ogc/2.0/gml-sf0\"",
         "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=application%2Fgml%2Bxml%3B%20version%3D3.2%3B%20profile%3D%22http%3A%2F%2Fwww.opengis.net%2Fdef%2Fprofile%2Fogc%2F2.0%2Fgml-sf0%22"
      },
      {
         "rel": "describedby",
         "title": "Schema for Roads",
         "type": "application/xml",
         "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/schema"
      }
   ]
}
```

#### jsonld
```jsonld
{
  "id": "roadl_1m",
  "title": "Roads",
  "extent": {
    "spatial": {
      "bbox": [
        [
          -179.999420166016,
          -54.88802337646479,
          179.9999,
          74.740592956543
        ]
      ],
      "crs": "http://www.opengis.net/def/crs/OGC/1.3/CRS84"
    },
    "temporal": {
      "interval": [
        [
          "2017-01-01T00:00:00Z",
          "2017-12-31T23:59:59Z"
        ]
      ],
      "trs": "http://www.opengis.net/def/uom/ISO-8601/0/Gregorian"
    }
  },
  "links": [
    {
      "rel": "self",
      "title": "This document",
      "type": "application/json",
      "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=application%2Fjson"
    },
    {
      "rel": "alternate",
      "title": "This document as HTML",
      "type": "text/html",
      "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=text%2Fhtml"
    },
    {
      "rel": "items",
      "title": "Roads",
      "type": "application/geo+json",
      "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=application%2Fgeo%2Bjson"
    },
    {
      "rel": "items",
      "title": "Roads",
      "type": "text/html",
      "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=text%2Fhtml"
    },
    {
      "rel": "items",
      "title": "Roads",
      "type": "application/gml+xml;version=3.2;profile=\"http://www.opengis.net/def/profile/ogc/2.0/gml-sf0\"",
      "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=application%2Fgml%2Bxml%3B%20version%3D3.2%3B%20profile%3D%22http%3A%2F%2Fwww.opengis.net%2Fdef%2Fprofile%2Fogc%2F2.0%2Fgml-sf0%22"
    },
    {
      "rel": "describedby",
      "title": "Schema for Roads",
      "type": "application/xml",
      "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/schema"
    }
  ],
  "@context": "https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/context.jsonld"
}
```

#### ttl
```ttl
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

[] rdfs:label "Roads" .


```

## Schema

```yaml
$comment: Adapted from https://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/collection.yaml
type: object
required:
- id
- links
properties:
  id:
    description: identifier of the collection used, for example, in URIs
    type: string
    example: address
  title:
    description: human readable title of the collection
    type: string
    example: address
  description:
    description: a description of the features in the collection
    type: string
    example: An address.
  links:
    type: array
    items:
      $ref: https://opengeospatial.github.io/bblocks/annotated-schemas/ogc-utils/json-link/schema.yaml
    example:
    - href: http://data.example.com/buildings
      rel: item
    - href: http://example.com/concepts/buildings.html
      rel: describedby
      type: text/html
  extent:
    $ref: https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/extent/schema.yaml
  itemType:
    description: indicator about the type of the items in the collection (the default
      value is 'feature').
    type: string
    default: feature
  crs:
    description: the list of coordinate reference systems supported by the service
    type: array
    items:
      type: string
    default:
    - http://www.opengis.net/def/crs/OGC/1.3/CRS84
    example:
    - http://www.opengis.net/def/crs/OGC/1.3/CRS84
    - http://www.opengis.net/def/crs/EPSG/0/4326

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/schema.yaml)


# JSON-LD Context

```jsonld
{
  "@context": {
    "href": {
      "@type": "@id",
      "@id": "oa:hasTarget"
    },
    "rel": {
      "@context": {
        "@base": "http://www.iana.org/assignments/relation/"
      },
      "@id": "http://www.iana.org/assignments/relation",
      "@type": "@id"
    },
    "type": "dct:type",
    "hreflang": "dct:language",
    "title": "rdfs:label",
    "length": "dct:extent",
    "oa": "http://www.w3.org/ns/oa#",
    "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
    "dct": "http://purl.org/dc/terms/",
    "@version": 1.1
  }
}
```

You can find the full JSON-LD context here:
[context.jsonld](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/context.jsonld)

## Sources

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-features](https://github.com/ogcincubator/bblocks-ogcapi-features)
* Path: `_sources/v1/schemas/collection`

