swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/event/{page}:
    get:
      summary: Get Admin Event Page
      description: Get admin event page.
      operationId: getApiV1AdminEventPage
      x-api-path-slug: apiv1admineventpage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.cityId
      - in: query
        name: request.from
      - in: query
        name: request.isRecommended
      - in: query
        name: request.placeId
      - in: query
        name: request.placeName
      - in: query
        name: request.query
      - in: query
        name: request.status
      - in: query
        name: request.to
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Page
  /api/v1/admin/place/{page}:
    get:
      summary: Get Admin Place Page
      description: Get admin place page.
      operationId: getApiV1AdminPlacePage
      x-api-path-slug: apiv1adminplacepage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.cityId
      - in: query
        name: request.isRecommended
      - in: query
        name: request.query
      - in: query
        name: request.status
      - in: query
        name: request.url
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Place
      - Page
  /api/v1/admin/placeReview/{page}:
    get:
      summary: Get Admin Placereview Page
      description: Get admin placereview page.
      operationId: getApiV1AdminPlacereviewPage
      x-api-path-slug: apiv1adminplacereviewpage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.placeName
      - in: query
        name: request.status
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Placereview
      - Page
  /api/v1/admin/promocode/{page}:
    get:
      summary: Get Admin Promocode Page
      description: Get admin promocode page.
      operationId: getApiV1AdminPromocodePage
      x-api-path-slug: apiv1adminpromocodepage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.used
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Promocode
      - Page
  /api/v1/art/search/{page}:
    post:
      summary: Post Art Search Page
      description: Post art search page.
      operationId: postApiV1ArtSearchPage
      x-api-path-slug: apiv1artsearchpage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Art
      - Search
      - Page
  /api/v1/gigme/artist/search/{page}:
    post:
      summary: Post Gigme Artist Search Page
      description: Post gigme artist search page.
      operationId: postApiV1GigmeArtistSearchPage
      x-api-path-slug: apiv1gigmeartistsearchpage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Artist
      - Search
      - Page
  /api/v1/gigme/event/previews/{page}:
    post:
      summary: Post Gigme Event Previews Page
      description: Post gigme event previews page.
      operationId: postApiV1GigmeEventPreviewsPage
      x-api-path-slug: apiv1gigmeeventpreviewspage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: preview
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Previews
      - Page
  /api/v1/gigme/event/{page}:
    post:
      summary: Post Gigme Event Page
      description: Post gigme event page.
      operationId: postApiV1GigmeEventPage
      x-api-path-slug: apiv1gigmeeventpage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Page
  /api/v1/gigme/place/{placeId}/reviews/{page}/{pageSize}:
    get:
      summary: Get Gigme Place Placeid Reviews Page Pagesize
      description: Get gigme place placeid reviews page pagesize.
      operationId: getApiV1GigmePlacePlaceReviewsPagePagesize
      x-api-path-slug: apiv1gigmeplaceplaceidreviewspagepagesize-get
      parameters:
      - in: path
        name: page
      - in: path
        name: pageSize
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Place
      - Placeid
      - Reviews
      - Page
      - Pagesize
  /api/v1/place/{placeId}/reviews/{page}/{pageSize}:
    get:
      summary: Get Place Placeid Reviews Page Pagesize
      description: Get place placeid reviews page pagesize.
      operationId: getApiV1PlacePlaceReviewsPagePagesize
      x-api-path-slug: apiv1placeplaceidreviewspagepagesize-get
      parameters:
      - in: path
        name: page
      - in: path
        name: pageSize
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Place
      - Placeid
      - Reviews
      - Page
      - Pagesize
  /api/v1/message/chats/{pageNumber}/{search}:
    get:
      summary: Get Message Chats Pagenumber Search
      description: Get message chats pagenumber search.
      operationId: getApiV1MessageChatsPagenumberSearch
      x-api-path-slug: apiv1messagechatspagenumbersearch-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: pageNumber
      - in: path
        name: search
      - in: query
        name: unread
      responses:
        200:
          description: OK
      tags:
      - Message
      - Chats
      - Pagenumber
      - Search