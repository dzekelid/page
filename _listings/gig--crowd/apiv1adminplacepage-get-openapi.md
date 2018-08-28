---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Admin Place Page
  version: 1.0.0
  description: Get admin place page.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/event/{page}:
    get:
      summary: Get Admin Event Page
      description: Get admin event page.
      operationId: getApiV1AdminEventPage
      x-api-path-slug: apiv1admineventpage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.cityId
      - in: query
        name: request.from
      - in: query
        name: request.isRecommended
      - in: query
        name: request.placeId
      - in: query
        name: request.placeName
      - in: query
        name: request.query
      - in: query
        name: request.status
      - in: query
        name: request.to
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Page
  /api/v1/admin/place/{page}:
    get:
      summary: Get Admin Place Page
      description: Get admin place page.
      operationId: getApiV1AdminPlacePage
      x-api-path-slug: apiv1adminplacepage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.cityId
      - in: query
        name: request.isRecommended
      - in: query
        name: request.query
      - in: query
        name: request.status
      - in: query
        name: request.url
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Page
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