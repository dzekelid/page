---
swagger: "2.0"
x-collection-name: Healthcare.gov
x-complete: 1
info:
  title: Healthcare
  version: 1.0.0
host: www.healthcare.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blog/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Blog Pagename
      description: Returns pages content.
      operationId: getBlogPagenameMediatypeextension
      x-api-path-slug: blogpagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Blog
      - Pagename
  /es/blog/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Es Blog Pagename
      description: Returns pages content.
      operationId: getEsBlogPagenameMediatypeextension
      x-api-path-slug: esblogpagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Es
      - Blog
      - Pagename
  /es/glossary/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Es Glossary Pagename
      description: Returns pages content.
      operationId: getEsGlossaryPagenameMediatypeextension
      x-api-path-slug: esglossarypagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Es
      - Glossary
      - Pagename
  /es/question/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Es Question Pagename
      description: Returns pages content.
      operationId: getEsQuestionPagenameMediatypeextension
      x-api-path-slug: esquestionpagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Es
      - Question
      - Pagename
  /es/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Es Pagename
      description: Returns pages content.
      operationId: getEsPagenameMediatypeextension
      x-api-path-slug: espagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Es
      - Pagename
  /glossary/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Glossary Pagename
      description: Returns pages content.
      operationId: getGlossaryPagenameMediatypeextension
      x-api-path-slug: glossarypagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Glossary
      - Pagename
  /question/{pageName}{mediaTypeExtension}:
    get:
      summary: Get Question Pagename
      description: Returns pages content.
      operationId: getQuestionPagenameMediatypeextension
      x-api-path-slug: questionpagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Question
      - Pagename
  /{pageName}{mediaTypeExtension}:
    get:
      summary: Get Pagename
      description: Returns pages content.
      operationId: getPagenameMediatypeextension
      x-api-path-slug: pagenamemediatypeextension-get
      parameters:
      - in: path
        name: mediaTypeExtension
        description: Omiting the param causes html to be returned
      - in: path
        name: pageName
      responses:
        200:
          description: OK
      tags:
      - Pagename
---