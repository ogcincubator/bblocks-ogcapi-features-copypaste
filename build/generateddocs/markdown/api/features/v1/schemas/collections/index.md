
# Schema for collections (Schema)

`ogc.api.features.v1.schemas.collections` *v0.1*

This building block corresponds to the schema for an OGC API Features collections

[*Status*](http://www.opengis.net/def/status): Under development

## Examples

### Object containing 3 collections
#### json
```json
{
   "links": [
      {
         "rel": "self",
         "title": "This document",
         "type": "application/json",
         "href": "http://www.acme.com/3.0/wfs/collections?f=application%2Fjson"
      },
      {
         "rel": "alternate",
         "title": "This document as XML",
         "type": "text/xml",
         "href": "http://www.acme.com/3.0/wfs/collections?f=text%2Fxml"
      },
      {
         "rel": "alternate",
         "title": "This document as HTML",
         "type": "text/html",
         "href": "http://www.acme.com/3.0/wfs/collections?f=text%2Fhtml"
      }
   ],
   "collections": [
      {
         "id": "aerofacp_1m",
         "title": "Airport Facilities Points",
         "extent":
         {
            "spatial":  {
               "bbox": [
                  [-179.878326416016,-54.9311103820801,
                    179.339859008789, 79.52944183349609]
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
         "links":
         [
            {
               "rel": "self",
               "title": "This collection",
               "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m"
            },
            {
               "rel": "items",
               "title": "Airport Facilities Points as GeoJSON",
               "type": "application/geo+json",
               "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m/items?f=application%2Fgeo%2Bjson"
            },
            {
               "rel": "items",
               "title": "Airport Facilities Points as HTML",
               "type": "text/html",
               "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m/items?f=text%2Fhtml"
            },
            {
               "rel": "items",
               "title": "Airport Facilities Points as GML",
               "type": "application/gml+xml;version=3.2;profile=\"http://www.opengis.net/def/profile/ogc/2.0/gml-sf0\"",
               "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m/items?f=application%2Fgml%2Bxml%3B%20version%3D3.2%3B%20profile%3D%22http%3A%2F%2Fwww.opengis.net%2Fdef%2Fprofile%2Fogc%2F2.0%2Fgml-sf0%22"
            },
            {
               "rel": "describedby",
               "title": "Schema for Airport Facilities Points",
               "type": "application/xml",
               "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m/schema"
            }
         ]
      },
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
               "title": "This collection",
               "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m"
            },
            {
               "rel": "items",
               "title": "Roads as GeoJSON",
               "type": "application/geo+json",
               "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=application%2Fgeo%2Bjson"
            },
            {
               "rel": "items",
               "title": "Roads as HTML",
               "type": "text/html",
               "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=text%2Fhtml"
            },
            {
               "rel": "items",
               "title": "Roads as GML",
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
      },
      {
         "id": "inwatera_1m",
         "title": "Inland Water Areas",
         "extent":
         {
            "spatial":  {
               "bbox": [
                  [-179.999420166016, -70.91725158691409,
                    179.9999, 83.57595062255859]
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
               "title": "This collection",
               "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m"
            },
            {
               "rel": "items",
               "title": "Inland Water Areas as GeoJSON",
               "type": "application/geo+json",
               "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m/items?f=application%2Fgeo%2Bjson"
            },
            {
               "rel": "items",
               "title": "Inland Water Areas as HTML",
               "type": "text/html",
               "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m/items?f=text%2Fhtml"
            },
            {
               "rel": "items",
               "title": "Inland Water Areas as GML",
               "type": "application/gml+xml; version=3.2;profile=\"http://www.opengis.net/def/profile/ogc/2.0/gml-sf0\"",
               "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m/items?f=application%2Fgml%2Bxml%2B%20version%2D3.2%2B%20profile%2Dhttp:%2F%2Fwww.opengis.net%2Fdef%2Fprofile%2Fogc%2F2.0%2Fgml-sf0"
            },
            {
               "rel": "describedby",
               "title": "Schema for Inland Water Areas",
               "type": "application/xml",
               "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m/schema"
            }
         ]
      }
   ]
}

```

#### jsonld
```jsonld
{
  "@context": "https://ogcincubator.github.io/bblocks-ogcapi-features-copypaste/build/annotated/api/features/v1/schemas/collections/context.jsonld",
  "links": [
    {
      "rel": "self",
      "title": "This document",
      "type": "application/json",
      "href": "http://www.acme.com/3.0/wfs/collections?f=application%2Fjson"
    },
    {
      "rel": "alternate",
      "title": "This document as XML",
      "type": "text/xml",
      "href": "http://www.acme.com/3.0/wfs/collections?f=text%2Fxml"
    },
    {
      "rel": "alternate",
      "title": "This document as HTML",
      "type": "text/html",
      "href": "http://www.acme.com/3.0/wfs/collections?f=text%2Fhtml"
    }
  ],
  "collections": [
    {
      "id": "aerofacp_1m",
      "title": "Airport Facilities Points",
      "extent": {
        "spatial": {
          "bbox": [
            [
              -179.878326416016,
              -54.9311103820801,
              179.339859008789,
              79.5294418334961
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
          "title": "This collection",
          "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m"
        },
        {
          "rel": "items",
          "title": "Airport Facilities Points as GeoJSON",
          "type": "application/geo+json",
          "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m/items?f=application%2Fgeo%2Bjson"
        },
        {
          "rel": "items",
          "title": "Airport Facilities Points as HTML",
          "type": "text/html",
          "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m/items?f=text%2Fhtml"
        },
        {
          "rel": "items",
          "title": "Airport Facilities Points as GML",
          "type": "application/gml+xml;version=3.2;profile=\"http://www.opengis.net/def/profile/ogc/2.0/gml-sf0\"",
          "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m/items?f=application%2Fgml%2Bxml%3B%20version%3D3.2%3B%20profile%3D%22http%3A%2F%2Fwww.opengis.net%2Fdef%2Fprofile%2Fogc%2F2.0%2Fgml-sf0%22"
        },
        {
          "rel": "describedby",
          "title": "Schema for Airport Facilities Points",
          "type": "application/xml",
          "href": "http://www.acme.com/3.0/wfs/collections/aerofacp_1m/schema"
        }
      ]
    },
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
          "title": "This collection",
          "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m"
        },
        {
          "rel": "items",
          "title": "Roads as GeoJSON",
          "type": "application/geo+json",
          "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=application%2Fgeo%2Bjson"
        },
        {
          "rel": "items",
          "title": "Roads as HTML",
          "type": "text/html",
          "href": "http://www.acme.com/3.0/wfs/collections/roadl_1m/items?f=text%2Fhtml"
        },
        {
          "rel": "items",
          "title": "Roads as GML",
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
    },
    {
      "id": "inwatera_1m",
      "title": "Inland Water Areas",
      "extent": {
        "spatial": {
          "bbox": [
            [
              -179.999420166016,
              -70.91725158691409,
              179.9999,
              83.5759506225586
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
          "title": "This collection",
          "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m"
        },
        {
          "rel": "items",
          "title": "Inland Water Areas as GeoJSON",
          "type": "application/geo+json",
          "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m/items?f=application%2Fgeo%2Bjson"
        },
        {
          "rel": "items",
          "title": "Inland Water Areas as HTML",
          "type": "text/html",
          "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m/items?f=text%2Fhtml"
        },
        {
          "rel": "items",
          "title": "Inland Water Areas as GML",
          "type": "application/gml+xml; version=3.2;profile=\"http://www.opengis.net/def/profile/ogc/2.0/gml-sf0\"",
          "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m/items?f=application%2Fgml%2Bxml%2B%20version%2D3.2%2B%20profile%2Dhttp:%2F%2Fwww.opengis.net%2Fdef%2Fprofile%2Fogc%2F2.0%2Fgml-sf0"
        },
        {
          "rel": "describedby",
          "title": "Schema for Inland Water Areas",
          "type": "application/xml",
          "href": "http://www.acme.com/3.0/wfs/collections/inwatera_1m/schema"
        }
      ]
    }
  ]
}
```

#### ttl
```ttl


```

## Schema

```yaml
$comment: Adapted from https://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/collections.yaml
type: object
properties:
  links:
    type: array
    items:
      $ref: https://opengeospatial.github.io/bblocks/annotated-schemas/ogc-utils/json-link/schema.yaml
  collections:
    type: array
    items:
      $ref: https://ogcincubator.github.io/bblocks-ogcapi-features-copypaste/build/annotated/api/features/v1/schemas/collection/schema.yaml

```

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-features-copypaste/build/annotated/api/features/v1/schemas/collections/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-features-copypaste/build/annotated/api/features/v1/schemas/collections/schema.yaml)


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
[context.jsonld](https://ogcincubator.github.io/bblocks-ogcapi-features-copypaste/build/annotated/api/features/v1/schemas/collections/context.jsonld)

## Sources

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-features-copypaste](https://github.com/ogcincubator/bblocks-ogcapi-features-copypaste)
* Path: `_sources/v1/schemas/collections`

