---
swagger: "2.0"
x-collection-name: Google Slides
x-complete: 1
info:
  title: Google Slides
  description: an-api-for-creating-and-editing-google-slides-presentations-
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
---