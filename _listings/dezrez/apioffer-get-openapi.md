---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Gets a paged amount of offerss.
  version: 1.0.0
  description: Gets a paged amount of offerss..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/stats/RecordVisit/{pageType}/{entityId}:
    post:
      summary: Record and timestamp a visit to a 'page' on Rezi.
      description: Record and timestamp a visit to a 'page' on rezi..
      operationId: Stats_RecordVisitBypageTypeByentityIdByroleId
      x-api-path-slug: apistatsrecordvisitpagetypeentityid-post
      parameters:
      - in: path
        name: entityId
        description: The relative entitiyId e
      - in: path
        name: pageType
        description: GroupHub, PropertyHub, MarketingHub, PersonHub, SalesProgressionHub
          or PreTenancyHub
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
        description: The RoleId if applicable (can be null if omitted)
      responses:
        200:
          description: OK
      tags:
      - Record
      - Timestamp
      - Visit
      - To
      - Page
      - "On"
      - Rezi
  /api/Offer:
    get:
      summary: Gets a paged amount of offerss.
      description: Gets a paged amount of offerss..
      operationId: Offer_GetBypageSizeBypageNumber
      x-api-path-slug: apioffer-get
      parameters:
      - in: query
        name: pageNumber
        description: The page of offerss to return
      - in: query
        name: pageSize
        description: The number of offerss to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Paged
      - Amount
      - Of
      - Offerss
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