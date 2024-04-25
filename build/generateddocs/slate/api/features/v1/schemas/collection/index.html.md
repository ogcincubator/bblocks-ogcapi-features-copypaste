---
title: Schema for collection (Schema)

language_tabs:
  - json: JSON
  - jsonld: JSON-LD
  - turtle: RDF/Turtle

toc_footers:
  - Version 0.1
  - <a href='#'>Schema for collection</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: Schema for collection (Schema)
---


# Schema for collection `ogc.api.features.v1.schemas.collection`

This building block corresponds to the schema for an OGC API Features collection

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong><a href="https://github.com/ogcincubator/bblocks-ogcapi-features/blob/master/build/tests/api/features/v1/schemas/collection/" target="_blank">valid</a></strong>
</aside>

# Examples

## Road collection



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

<blockquote class="lang-specific json">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/tests/api/features/v1/schemas/collection/example_1_1.json">Open in new window</a>
    <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=json&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Ftests%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fcollection%2Fexample_1_1.json&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on JSON Viewer</a></p>
</blockquote>




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

<blockquote class="lang-specific jsonld">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/tests/api/features/v1/schemas/collection/example_1_1.jsonld">Open in new window</a>
    <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Ftests%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fcollection%2Fexample_1_1.jsonld">View on JSON-LD Playground</a>
</blockquote>




```turtle
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

[] rdfs:label "Roads" .


```

<blockquote class="lang-specific turtle">
  <p class="example-links">
    <a target="_blank" href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/tests/api/features/v1/schemas/collection/example_1_1.ttl">Open in new window</a>
</blockquote>



# JSON Schema

```yaml--schema
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

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Fannotated%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fcollection%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/schema.json</a>


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

> <a target="_blank" href="https://json-ld.org/playground/#json-ld=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Fannotated%2Fapi%2Ffeatures%2Fv1%2Fschemas%2Fcollection%2Fcontext.jsonld">View on JSON-LD Playground</a>

You can find the full JSON-LD context here:
<a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/context.jsonld" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/collection/context.jsonld</a>

# References

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-ogcapi-features" target="_blank">https://github.com/ogcincubator/bblocks-ogcapi-features</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-ogcapi-features/blob/HEAD/_sources/v1/schemas/collection" target="_blank">_sources/v1/schemas/collection</a></code>

