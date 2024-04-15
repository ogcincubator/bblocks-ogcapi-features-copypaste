---
title: Schema for limit (Parameter)

toc_footers:
  - Version 0.1
  - <a href='#'>Schema for limit</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: Schema for limit (Parameter)
---


# Schema for limit `ogc.api.features.v1.parameters.featureId`

This building block corresponds to the schema for an OGC API Records featureId

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong>valid</strong>
</aside>


# JSON Schema

```yaml--schema
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

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Fannotated%2Fapi%2Ffeatures%2Fv1%2Fparameters%2FfeatureId%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/featureId/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/featureId/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/featureId/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/featureId/schema.json</a>

# References

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-ogcapi-features" target="_blank">https://github.com/ogcincubator/bblocks-ogcapi-features</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-ogcapi-features/blob/HEAD/_sources/v1/parameters/featureId" target="_blank">_sources/v1/parameters/featureId</a></code>

