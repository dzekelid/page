---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Delete Page Tabs Tab
  description: Deletes an installed profile tab (where is_permanent is not true) for
    a page
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
    post:
      summary: Post Page Settings
      description: The page's post permission settings
      operationId: postPageSettings
      x-api-path-slug: pagesettings-post
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: setting
        description: 'Which single setting to update: USERS_CAN_POST, USERS_CAN_POST_PHOTOS,
          USERS_CAN_TAG_PHOTOS, USERS_CAN_POST_VIDEOS'
      - in: query
        name: value
        description: Connect to the social network with the Graph API
      responses:
        200:
          description: OK
      tags:
      - Page
      - Settings
  /{page}/tagged:
    get:
      summary: Get Page Tagged
      description: The photos, videos, and posts in which this page has been tagged
      operationId: getPageTagged
      x-api-path-slug: pagetagged-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tagged
  /{page}/links:
    get:
      summary: Get Page Links
      description: The page's posted links
      operationId: getPageLinks
      x-api-path-slug: pagelinks-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Links
    post:
      summary: Post Page Links
      description: Posts a link on the page
      operationId: postPageLinks
      x-api-path-slug: pagelinks-post
      parameters:
      - in: query
        name: link
        description: Link URL
      - in: query
        name: message
        description: Link message
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Links
  /{page}/photos:
    get:
      summary: Get Page Photos
      description: The photos contained on this page
      operationId: getPagePhotos
      x-api-path-slug: pagephotos-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Photos
    post:
      summary: Post Page Photos
      description: Adds a photo to the page
      operationId: postPagePhotos
      x-api-path-slug: pagephotos-post
      parameters:
      - in: query
        name: message
        description: Photo description
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Photos
  /{page}/groups:
    get:
      summary: Get Page Groups
      description: The groups this page is a member of
      operationId: getPageGroups
      x-api-path-slug: pagegroups-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Groups
  /{page}/albums:
    get:
      summary: Get Page Albums
      description: The photo albums this Page has uploaded
      operationId: getPageAlbums
      x-api-path-slug: pagealbums-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Albums
  /{page}/statuses:
    get:
      summary: Get Page Statuses
      description: The page's status updates
      operationId: getPageStatuses
      x-api-path-slug: pagestatuses-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Statuses
    post:
      summary: Post Page Statuses
      description: Posts a status message on the page
      operationId: postPageStatuses
      x-api-path-slug: pagestatuses-post
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
      - Statuses
  /{page}/videos:
    get:
      summary: Get Page Veos
      description: The videos contained on this page
      operationId: getPageVeos
      x-api-path-slug: pagevideos-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Videos
    post:
      summary: Post Page Veos
      description: Publishes a video to the page
      operationId: postPageVeos
      x-api-path-slug: pagevideos-post
      parameters:
      - in: query
        name: description
        description: Video description
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: title
        description: Video title
      responses:
        200:
          description: OK
      tags:
      - Page
      - Videos
  /{page}/notes:
    get:
      summary: Get Page Notes
      description: The notes contained on this page
      operationId: getPageNotes
      x-api-path-slug: pagenotes-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Notes
    post:
      summary: Post Page Notes
      description: Creates a note on the page
      operationId: postPageNotes
      x-api-path-slug: pagenotes-post
      parameters:
      - in: query
        name: message
        description: Note content
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: subject
        description: The subject of the Note
      responses:
        200:
          description: OK
      tags:
      - Page
      - Notes
  /{page}/posts:
    get:
      summary: Get Page Adds
      description: The page's own posts
      operationId: getPageAdds
      x-api-path-slug: pageposts-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Posts
  /{page}/events:
    get:
      summary: Get Page Events
      description: The events the Page is attending
      operationId: getPageEvents
      x-api-path-slug: pageevents-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Events
    post:
      summary: Post Page Events
      description: Creates an event for the page
      operationId: postPageEvents
      x-api-path-slug: pageevents-post
      parameters:
      - in: query
        name: end_time
        description: Event end time
      - in: query
        name: location
        description: Event location
      - in: query
        name: message
        description: Event description
      - in: query
        name: name
        description: Event name
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: privacy_type
        description: Event privacy setting
      - in: query
        name: start_time
        description: Event start time
      responses:
        200:
          description: OK
      tags:
      - Page
      - Events
  /{page}/checkins:
    get:
      summary: Get Page Checkins
      description: Checkins made to this Place Page by the current user, and friends
        of the current user
      operationId: getPageCheckins
      x-api-path-slug: pagecheckins-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Checkins
  /{page}/tabs:
    get:
      summary: Get Page Tabs
      description: The page's profile tabs
      operationId: getPageTabs
      x-api-path-slug: pagetabs-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tabs
    post:
      summary: Post Page Tabs
      description: Installs a profile tab at the end of the current list of installed
        tabs for the page
      operationId: postPageTabs
      x-api-path-slug: pagetabs-post
      parameters:
      - in: query
        name: app_id
        description: ID of the application for which to install the tab
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tabs
  /{page}/tabs/{tab}:
    post:
      summary: Post Page Tabs Tab
      description: Updates an installed profile tab for a page
      operationId: postPageTabsTab
      x-api-path-slug: pagetabstab-post
      parameters:
      - in: query
        name: custom_name
        description: Name to be used for the tab
      - in: query
        name: is_non_connection_landing_tab
        description: Set this tab as the default landing tab for users who have not
          liked and are not admins of the Page
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: position
        description: Order in which the tab will appear on the profile
      - in: path
        name: tab
        description: Represents the ID of the tab
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tabs
      - Tab
    delete:
      summary: Delete Page Tabs Tab
      description: Deletes an installed profile tab (where is_permanent is not true)
        for a page
      operationId: deletePageTabsTab
      x-api-path-slug: pagetabstab-delete
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: path
        name: tab
        description: Represents the ID of the tab
      responses:
        200:
          description: OK
      tags:
      - Page
      - Tabs
      - Tab
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