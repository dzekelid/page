---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get a single page by its ID
  description: Get a single page by its id.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/pages/216307854.json:
    put:
      summary: update a page
      description: Update a page.
      operationId: putAdminPages216307854.json
      x-api-path-slug: adminpages216307854-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Update
      - Page
    delete:
      summary: Delete a page
      description: Delete a page.
      operationId: deleteAdminPages216307854.json
      x-api-path-slug: adminpages216307854-json-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Page
  /admin/pages.json:
    post:
      summary: Create a new page
      description: Create a new page.
      operationId: postAdminPages.json
      x-api-path-slug: adminpages-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Page
  /admin/pages/169722563.json:
    get:
      summary: Get a single page by its ID
      description: Get a single page by its id.
      operationId: getAdminPages169722563.json
      x-api-path-slug: adminpages169722563-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Page
      - By
      - Its
      - ID
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