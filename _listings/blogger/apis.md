---
name: Blogger
x-slug: blogger
description: Blogger is a blog-publishing service that allows multi-user blogs with
  time-stamped entries. It was developed by Pyra Labs, which was bought by Google
  in 2003. Generally, the blogs are hosted by Google at a subdomain of blogspot.com.
  Blogs can also be hosted in the registered custom domain of the blogger (like www.example.com).
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Page
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/apis.md
specificationVersion: "0.14"
apis:
- name: Blogger - Get Blog Pages
  x-api-slug: blogsblogidpages-get
  description: Retrieves the pages for a blog, optionally including non-LIVE statuses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blog, Google APIs, Content, CMS, Stack Network, API Service Provider, API
    Provider, Profiles, General Data, Relative Data, Pedestal
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpages-get-openapi.md
- name: Blogger - Add Blog Page
  x-api-slug: blogsblogidpages-post
  description: Add a page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blog, Google APIs, Content, CMS, Stack Network, API Service Provider, API
    Provider, Profiles, General Data, Relative Data, Pedestal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpages-post-openapi.md
- name: Blogger - Delete Blog Page
  x-api-slug: blogsblogidpagespageid-delete
  description: Delete a page by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blog, Google APIs, Content, CMS, Stack Network, API Service Provider, API
    Provider, Profiles, General Data, Relative Data, Pedestal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpagespageid-delete-openapi.md
- name: Blogger - Get Blog Page
  x-api-slug: blogsblogidpagespageid-get
  description: Gets one blog page by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blog, Google APIs, Content, CMS, Stack Network, API Service Provider, API
    Provider, Profiles, General Data, Relative Data, Pedestal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpagespageid-get-openapi.md
- name: Blogger - Update Blog Page
  x-api-slug: blogsblogidpagespageid-patch
  description: Update a page. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blog, Google APIs, Content, CMS, Stack Network, API Service Provider, API
    Provider, Profiles, General Data, Relative Data, Pedestal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpagespageid-patch-openapi.md
- name: Blogger - Update Blog Page
  x-api-slug: blogsblogidpagespageid-put
  description: Update a page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blog, Google APIs, Content, CMS, Stack Network, API Service Provider, API
    Provider, Profiles, General Data, Relative Data, Pedestal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpagespageid-put-openapi.md
- name: Blogger - Publish Blog Page
  x-api-slug: blogsblogidpagespageidpublish-post
  description: Publishes a draft page.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blog, Google APIs, Content, CMS, Stack Network, API Service Provider, API
    Provider, Profiles, General Data, Relative Data, Pedestal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpagespageidpublish-post-openapi.md
- name: Blogger - Revert Blog Page
  x-api-slug: blogsblogidpagespageidrevert-post
  description: Revert a published or scheduled page to draft state.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/blogger-icon.png
  humanURL: https://www.blogger.com
  baseURL: ://www.googleapis.com//blogger/v3
  tags: Blog, Google APIs, Content, CMS, Stack Network, API Service Provider, API
    Provider, Profiles, General Data, Relative Data, Pedestal
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/page/master/_listings/blogger/blogsblogidpagespageidrevert-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://blockchain.api.gallery.streamdata.io
- type: x-api-stack
  url: http://blogger.stack.network
- type: x-blog
  url: https://blogger.googleblog.com/
- type: x-website
  url: https://www.blogger.com
- type: x-blog-rss
  url: http://buzz.blogger.com/atom.xml
- type: x-developer
  url: https://developers.google.com/blogger/
- type: x-twitter
  url: https://twitter.com/Blogger
- type: x-getting-started
  url: https://developers.google.com/blogger/docs/3.0/getting_started
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---