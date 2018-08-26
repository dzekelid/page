{
  "info": {
    "name": "One Note Get Pages Pageid Content",
    "_postman_id": "abcc37aa-56fd-48f0-a3b6-4354d0a91714",
    "description": "Returns HTML content of the specified page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pages",
      "item": [
        {
          "id": "48889bd5-25c9-4a79-8068-4689e567f5cf",
          "name": "getPagesPageContent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.onenote.com",
              "path": [
                "api",
                "v1.0",
                "me",
                "notes",
                "pages/:pageId/content"
              ],
              "query": [
                {
                  "key": "includeIDs",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "pageId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "Required: indicates type of content returned in the response",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns HTML content of the specified page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc9aa044-1fef-4b88-9a2c-b620ee1adcee"
            }
          ]
        }
      ]
    }
  ]
}