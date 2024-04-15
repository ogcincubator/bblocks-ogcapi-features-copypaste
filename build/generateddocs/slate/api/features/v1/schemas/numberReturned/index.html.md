---
title: Schema for numberReturned (Datatype)

toc_footers:
  - Version 0.1
  - <a href='#'>Schema for numberReturned</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: Schema for numberReturned (Datatype)
---


# Schema for numberReturned `ogc.api.features.v1.schemas.numberReturned`

The number of features in the feature collection

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong>valid</strong>
</aside>

# Description

A server may omit this information in a response, if the information
about the number of features is not known or difficult to compute.

If the value is provided, the value shall be identical to the number
of items in the "features" array.

# JSON Schema

```yaml--schema
description: 'The number of features in the feature collection.


  A server may omit this information in a response, if the information

  about the number of features is not known or difficult to compute.


  If the value is provided, the value shall be identical to the number

  of items in the "features" array.'
type: integer
minimum: 0
example: 10

```

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Fannotated%2Fapi%2Ffeatures%2Fv1%2Fschemas%2FnumberReturned%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/numberReturned/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/numberReturned/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/numberReturned/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/schemas/numberReturned/schema.json</a>

# References

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-ogcapi-features" target="_blank">https://github.com/ogcincubator/bblocks-ogcapi-features</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-ogcapi-features/blob/HEAD/_sources/v1/schemas/numberReturned" target="_blank">_sources/v1/schemas/numberReturned</a></code>

