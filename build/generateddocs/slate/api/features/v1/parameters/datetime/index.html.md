---
title: Schema for datetime (Parameter)

toc_footers:
  - Version 0.1
  - <a href='#'>Schema for datetime</a>
  - <a href='https://blocks.ogc.org/register.html'>Building Blocks register</a>

search: true

code_clipboard: true

meta:
  - name: Schema for datetime (Parameter)
---


# Schema for datetime `ogc.api.features.v1.parameters.datetime`

This building block corresponds to the schema for an OGC API Records datetime

<p class="status">
    <span data-rainbow-uri="http://www.opengis.net/def/status">Status</span>:
    <a href="http://www.opengis.net/def/status/under-development" target="_blank" data-rainbow-uri>Under development</a>
</p>

<aside class="success">
This building block is <strong>valid</strong>
</aside>


# JSON Schema

```yaml--schema
name: datetime
in: query
description: 'Either a date-time or an interval. Date and time expressions adhere
  to RFC 3339.

  Intervals may be bounded or half-bounded (double-dots at start or end).


  Examples:


  * A date-time: "2018-02-12T23:20:50Z"

  * A bounded interval: "2018-02-12T00:00:00Z/2018-03-18T12:31:12Z"

  * Half-bounded intervals: "2018-02-12T00:00:00Z/.." or "../2018-03-18T12:31:12Z"


  Only features that have a temporal property that intersects the value of

  `datetime` are selected.


  If a feature has multiple temporal properties, it is the decision of the

  server whether only a single temporal property is used to determine

  the extent or all relevant temporal properties.'
required: false
schema:
  type: string
style: form
explode: false

```

> <a target="_blank" href="https://avillar.github.io/TreedocViewer/?dataParser=yaml&amp;dataUrl=https%3A%2F%2Fogcincubator.github.io%2Fbblocks-ogcapi-features%2Fbuild%2Fannotated%2Fapi%2Ffeatures%2Fv1%2Fparameters%2Fdatetime%2Fschema.yaml&amp;expand=2&amp;option=%7B%22showTable%22%3A+false%7D">View on YAML Viewer</a>

Links to the schema:

* YAML version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/datetime/schema.yaml" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/datetime/schema.yaml</a>
* JSON version: <a href="https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/datetime/schema.json" target="_blank">https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/datetime/schema.json</a>

# References

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: <a href="https://github.com/ogcincubator/bblocks-ogcapi-features" target="_blank">https://github.com/ogcincubator/bblocks-ogcapi-features</a>
* Path:
<code><a href="https://github.com/ogcincubator/bblocks-ogcapi-features/blob/HEAD/_sources/v1/parameters/datetime" target="_blank">_sources/v1/parameters/datetime</a></code>

