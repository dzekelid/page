---
swagger: "2.0"
x-collection-name: Blogger
x-complete: 0
info:
  title: Blogger API Get Blog Pages
  description: Retrieves the pages for a blog, optionally including non-LIVE statuses.
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /blogger/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blogs/{blogId}/pages:
    get:
      summary: Get Blog Pages
      description: Retrieves the pages for a blog, optionally including non-LIVE statuses.
      operationId: blogger.pages.list
      x-api-path-slug: blogsblogidpages-get
      parameters:
      - in: path
        name: blogId
        description: ID of the blog to fetch Pages from
      - in: query
        name: fetchBodies
        description: Whether to retrieve the Page bodies
      - in: query
        name: maxResults
        description: Maximum number of Pages to fetch
      - in: query
        name: pageToken
        description: Continuation token if the request is paged
      - in: query
        name: status
      - in: query
        name: view
        description: Access level with which to view the returned result
      responses:
        200:
          description: OK
      tags:
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