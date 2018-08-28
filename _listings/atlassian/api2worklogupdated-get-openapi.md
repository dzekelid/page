---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get IDs of updated worklogs
  description: "Returns a list of IDs and update timestamps for worklogs updated after
    a date and time.  \n  \nThis resource is paginated, with a limit of 1000 worklogs
    per page. Each page lists worklogs from oldest to youngest. If the number of items
    in the date range exceeds 1000, `until` indicates the timestamp of the youngest
    item on the page. Also, `nextPage` provides the URL for the next page of worklogs.
    The `lastPage` parameter is set to true on the last page of worklogs.  \n  \nThis
    resource does not return worklogs updated during the minute preceding the request.
    \ \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**
    Permission to access Jira."
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /content/{id}/pagehierarchy/copy:
    post:
      summary: Copy page hierarchy
      description: |-
        Copy page hierarchy allows the copying of an entire hierarchy of pages and their associated properties, permissions and attachments.
         The id path parameter refers to the content id of the page to copy, and the new parent of this copied page is defined using the destinationPageId in the request body.
         The titleOptions object defines the rules of renaming page titles during the copy;
         for example, search and replace can be used in conjunction to rewrite the copied page titles.

         Response example:
         <pre><code>
         {
              "id" : "1180606",
              "links" : {
                   "status" : "/rest/api/longtask/1180606"
              }
         }
         </code></pre>
         Use the /longtask/<taskId> REST API to get the copy task status.
      operationId: com.atlassian.confluence.plugins.restapi.resources.PageHierarchyResource.copyPageHierarchy_post
      x-api-path-slug: contentidpagehierarchycopy-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Copy
      - Page
      - Hierarchy
  /api/2/worklog/deleted:
    get:
      summary: Get IDs of deleted worklogs
      description: "Returns a list of IDs and delete timestamps for worklogs deleted
        after a date and time.  \n  \nThis resource is paginated, with a limit of
        1000 worklogs per page. Each page lists worklogs from oldest to youngest.
        If the number of items in the date range exceeds 1000, `until` indicates the
        timestamp of the youngest item on the page. Also, `nextPage` provides the
        URL for the next page of worklogs. The `lastPage` parameter is set to true
        on the last page of worklogs.  \n  \nThis resource does not return worklogs
        deleted during the minute preceding the request.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to access Jira."
      operationId: com.atlassian.jira.rest.v2.issue.worklog.WorklogResource.getIdsOfWorklogsDeletedSince_get
      x-api-path-slug: api2worklogdeleted-get
      parameters:
      - in: query
        name: since
        description: The date and time, in UNIX timestamp format, after which deleted
          worklogs are returned
      responses:
        200:
          description: OK
      tags:
      - IDs
      - Of
      - Deleted
      - Worklogs
  /api/2/worklog/updated:
    get:
      summary: Get IDs of updated worklogs
      description: "Returns a list of IDs and update timestamps for worklogs updated
        after a date and time.  \n  \nThis resource is paginated, with a limit of
        1000 worklogs per page. Each page lists worklogs from oldest to youngest.
        If the number of items in the date range exceeds 1000, `until` indicates the
        timestamp of the youngest item on the page. Also, `nextPage` provides the
        URL for the next page of worklogs. The `lastPage` parameter is set to true
        on the last page of worklogs.  \n  \nThis resource does not return worklogs
        updated during the minute preceding the request.  \n  \n**[Permissions](https://confluence.atlassian.com/x/FQiiLQ)
        required:** Permission to access Jira."
      operationId: com.atlassian.jira.rest.v2.issue.worklog.WorklogResource.getIdsOfWorklogsModifiedSince_get
      x-api-path-slug: api2worklogupdated-get
      parameters:
      - in: query
        name: expand
        description: Use [expand](https://developer
      - in: query
        name: since
        description: The date and time, in UNIX timestamp format, after which updated
          worklogs are returned
      responses:
        200:
          description: OK
      tags:
      - IDs
      - Of
      - Updated
      - Worklogs
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