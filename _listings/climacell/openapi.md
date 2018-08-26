---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 1
info:
  title: ClimaCell API
  description: the-climacell-rest-api-provides-access-to-high-resolution-weather-data-for-locations-across-the-u-s--with-global-data-coming-soon--it-uses-https-and-requires-an-access-token-key--the-api-requests-carry-query-parameters-and-the-responses-return-results-in-json-format-
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts:
    get:
      summary: Get Alerts
      description: |-
        ### List all Alerts

        Page through a list of all your alerts. You can specify the maximum number of results to be retuned, and from which result to start.
      operationId: -list-all-alertspage-through-a-list-of-all-your-alerts-you-can-specify-the-maximum-number-of-results
      x-api-path-slug: alerts-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of records to load
      - in: query
        name: offset
        description: The number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Alerts
---