---
swagger: "2.0"
x-collection-name: Bookeo
x-complete: 1
info:
  title: Bookeo
  version: 1.0.0
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
---