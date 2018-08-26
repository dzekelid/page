---
swagger: "2.0"
x-collection-name: OneNote
x-complete: 1
info:
  title: One Note
  description: easily-capture-content-into-onenote-with-this-rest-api-
  version: 1.0.0
host: www.onenote.com
basePath: /api/v1.0/me/notes/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /pages/{pageId}/content:
    get:
      summary: Get Pages Pageid Content
      description: Returns HTML content of the specified page.
      operationId: getPagesPageContent
      x-api-path-slug: pagespageidcontent-get
      parameters:
      - in: header
        name: Accept
        description: 'Required: indicates type of content returned in the response'
      - in: query
        name: Accept
        description: 'Required: indicates type of content returned in the response'
      - in: query
        name: includeIDs
        description: 'Optional: set to true to get generated IDs to use for PATCH
          operations'
      - in: path
        name: pageId
        description: Specifies the page whose content you want to retrieve
      responses:
        200:
          description: OK
      tags:
      - Pages
      - PageId
      - Content
    parameters:
      summary: Parameters Pages Pageid Content
      description: Parameters pages pageid content.
      operationId: parametersPagesPageContent
      x-api-path-slug: pagespageidcontent-parameters
      responses:
        200:
          description: OK
      tags:
      - Pages
      - PageId
      - Content
  /pages/{pageId}:
    delete:
      summary: Delete Pages Pageid
      description: Deletes the specified page.
      operationId: deletePagesPage
      x-api-path-slug: pagespageid-delete
      parameters:
      - in: path
        name: pageId
        description: Specifies the page to delete
      responses:
        200:
          description: OK
      tags:
      - Pages
      - PageId
    get:
      summary: Get Pages Pageid
      description: Returns the specified page.
      operationId: getPagesPage
      x-api-path-slug: pagespageid-get
      parameters:
      - in: query
        name: expand
        description: The navigation properties (parentNotebook or parentSection) to
          return inline in the response
      - in: path
        name: pageId
        description: Specifies the page to get
      - in: query
        name: pagelevel
        description: true, to return the level and order properties
      - in: query
        name: select
        description: The properties to return
      responses:
        200:
          description: OK
      tags:
      - Pages
      - PageId
    parameters:
      summary: Parameters Pages Pageid
      description: Parameters pages pageid.
      operationId: parametersPagesPage
      x-api-path-slug: pagespageid-parameters
      responses:
        200:
          description: OK
      tags:
      - Pages
      - PageId
  /pages/{pageId}/preview:
    get:
      summary: Get Pages Pageid Preview
      description: Returns preview text and (if there is one) a preview image for
        the specified page.
      operationId: getPagesPagePreview
      x-api-path-slug: pagespageidpreview-get
      parameters:
      - in: query
        name: Content-Type
        description: 'Required: indicates type of content being sent'
      - in: path
        name: pageId
        description: Specifies the page whose content you want to retrieve
      responses:
        200:
          description: OK
      tags:
      - Pages
      - PageId
      - Preview
---