---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Modifies the details of a Favorites page in Square Register.
  description: Modifies the details of a Favorites page in Square Register.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/{location_id}/pages:
    post:
      summary: Creates a Favorites page in Square Register.
      description: Creates a Favorites page in Square Register.
      operationId: CreatePage
      x-api-path-slug: v1location-idpages-post
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the location to create an item for
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Favorites
      - Page
      - In
      - Square
      - Register
  /v1/{location_id}/pages/{page_id}:
    delete:
      summary: Deletes an existing Favorites page and all of its cells.
      description: Deletes an existing Favorites page and all of its cells.
      operationId: DeletePage
      x-api-path-slug: v1location-idpagespage-id-delete
      parameters:
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to delete
      responses:
        200:
          description: OK
      tags:
      - S
      - Existing
      - Favorites
      - Page
      - ""
      - Of
      - Its
      - Cells
    put:
      summary: Modifies the details of a Favorites page in Square Register.
      description: Modifies the details of a Favorites page in Square Register.
      operationId: UpdatePage
      x-api-path-slug: v1location-idpagespage-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: location_id
        description: The ID of the Favorites pages associated location
      - in: path
        name: page_id
        description: The ID of the page to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Details
      - Of
      - Favorites
      - Page
      - In
      - Square
      - Register
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