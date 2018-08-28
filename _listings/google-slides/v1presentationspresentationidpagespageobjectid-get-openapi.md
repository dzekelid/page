---
swagger: "2.0"
x-collection-name: Google Slides
x-complete: 0
info:
  title: Google Slides API Get Presentation Page
  description: Gets the latest version of the specified page in the presentation.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: slides.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/presentations/{presentationId}/pages/{pageObjectId}:
    get:
      summary: Get Presentation Page
      description: Gets the latest version of the specified page in the presentation.
      operationId: slides.presentations.pages.get
      x-api-path-slug: v1presentationspresentationidpagespageobjectid-get
      parameters:
      - in: path
        name: pageObjectId
        description: The object ID of the page to retrieve
      - in: path
        name: presentationId
        description: The ID of the presentation to retrieve
      responses:
        200:
          description: OK
      tags:
      - Presentation
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