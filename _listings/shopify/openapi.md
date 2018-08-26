---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
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
---