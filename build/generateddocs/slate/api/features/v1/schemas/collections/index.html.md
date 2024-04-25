---
title: Schema for collections (Schema)

language_tabs:
  - json: JSON
  - jsonld: JSON-LD

toc_footers:
  - Version 0.1
  - <a href='#'>Schema for collections</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: Schema for collections (Schema)
---


# Schema for collections `ogc.api.features.v1.schemas.collections`

This building block corresponds to the schema for an OGC API Features collections

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="warning">
Validation for this building block has <strong><a href="https://github.com/ogcincubator/bblocks-ogcapi-features/blob/master/build/tests/api/features/v1/schemas/collections/" target="_blank">failed</a></strong>
</aside>

# Examples

## Object containing 3 collections



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

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/tests/api/features/v1/schemas/collections/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Ftests%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fcollections%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>




```jsonld
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
  ],
  "@context": "https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collections/context.jsonld"
}
```

<blockquote class="lang-specific jsonld">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/tests/api/features/v1/schemas/collections/example_1_1.jsonld">Open in new window</a>
    <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Ftests%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fcollections%2Fexample_1_1.jsonld">View on JSON-LD Playground</a>
</blockquote>




# JSON Schema

```yaml--schema
$comment: https://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/collections.yaml
type: object
properties:
  links:
    type: array
    items:
      $ref: https://opengeospatial.github.io/bblocks/annotated-schemas/ogc-utils/json-link/schema.yaml
  collections:
    type: array
    items:
      $ref: https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/schema.yaml

```

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Fannotated%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fcollections%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collections/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collections/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collections/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collections/schema.json</a>


# JSON-LD Context

```json--ldContext
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

> <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Fannotated%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fcollections%2Fcontext.jsonld">View on JSON-LD Playground</a>

You can find the full JSON-LD context here:
<a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collections/context.jsonld" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collections/context.jsonld</a>

# References

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-ogcapi-features" target="_blank">https://github.com/ogcincubator/bblocks-ogcapi-features</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-ogcapi-features/blob/HEAD/_sources/v1/schemas/collections" target="_blank">_sources/v1/schemas/collections</a></code>

