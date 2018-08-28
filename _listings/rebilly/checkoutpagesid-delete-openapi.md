---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Delete a Checkout Page
  description: Delete a Checkout Page with predefined identifier string
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /checkout-pages:
    post:
      summary: Create a Checkout Page
      description: Create a Checkout Page
      operationId: create-a-checkout-page
      x-api-path-slug: checkoutpages-post
      parameters:
      - in: body
        name: body
        description: Checkout Page resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Checkout
      - Page
  /checkout-pages/{id}:
    delete:
      summary: Delete a Checkout Page
      description: Delete a Checkout Page with predefined identifier string
      operationId: delete-a-checkout-page-with-predefined-identifier-string
      x-api-path-slug: checkoutpagesid-delete
      responses:
        200:
          description: OK
      tags:
      - Checkout
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