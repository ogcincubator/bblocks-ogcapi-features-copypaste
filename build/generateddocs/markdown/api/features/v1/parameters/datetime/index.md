
# Schema for datetime (Parameter)

`ogc.api.features.v1.parameters.datetime` *v0.1*

This building block corresponds to the schema for an OGC API Features datetime

[*Status*](http://www.opengis.net/def/status): Under development

## Schema

```yaml
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

Links to the schema:

* YAML version: [schema.yaml](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/datetime/schema.json)
* JSON version: [schema.json](https://ogcincubator.github.io/bblocks-ogcapi-features/build/annotated/api/features/v1/parameters/datetime/schema.yaml)

## Sources

* [OGC API Features - Part 1 - Core corrigendum](https://docs.ogc.org/is/17-069r4/17-069r4.html)

# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/bblocks-ogcapi-features](https://github.com/ogcincubator/bblocks-ogcapi-features)
* Path: `_sources/v1/parameters/datetime`

