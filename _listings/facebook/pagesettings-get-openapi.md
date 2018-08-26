---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Page Settings
  description: The page's post permission settings
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{page}:
    get:
      summary: Get Page
      description: Returns a Page
      operationId: getPage
      x-api-path-slug: page-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
  /{page}/feed:
    get:
      summary: Get Page Feed
      description: This page's wall
      operationId: getPageFeed
      x-api-path-slug: pagefeed-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Feed
    post:
      summary: Post Page Feed
      description: Posts a status message on this page's wall
      operationId: postPageFeed
      x-api-path-slug: pagefeed-post
      parameters:
      - in: query
        name: message
        description: Status Message content
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Feed
  /{page}/picture:
    get:
      summary: Get Page Picture
      description: The page's profile picture
      operationId: getPagePicture
      x-api-path-slug: pagepicture-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      responses:
        200:
          description: OK
      tags:
      - Page
      - Picture
  /{page}/settings:
    get:
      summary: Get Page Settings
      description: The page's post permission settings
      operationId: getPageSettings
      x-api-path-slug: pagesettings-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Settings
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