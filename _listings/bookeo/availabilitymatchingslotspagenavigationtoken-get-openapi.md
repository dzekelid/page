---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 0
info:
  title: Bookeo Navigate results of a matching slots search
  version: 1.0.0
  description: Navigate results of a matching slots search.
host: api.bookeo.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /availability/matchingslots/{pageNavigationToken}:
    get:
      summary: Navigate results of a matching slots search
      description: Navigate results of a matching slots search.
      operationId: getAvailabilityMatchingslotsPagenavigationtoken
      x-api-path-slug: availabilitymatchingslotspagenavigationtoken-get
      parameters:
      - in: path
        name: pageNavigationToken
      - in: query
        name: pageNumber
      responses:
        200:
          description: OK
      tags:
      - Availability
      - Matchingslots
      - PageNavigationToken
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---