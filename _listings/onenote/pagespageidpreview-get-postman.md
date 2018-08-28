{
  "info": {
    "name": "One Note Get Pages Pageid Preview",
    "_postman_id": "c31d8dac-aaba-4792-b83f-a982f4f1ff5b",
    "description": "Returns preview text and (if there is one) a preview image for the specified page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pages",
      "item": [
        {
          "id": "a3d11c64-eae5-4ce7-a698-448d470381bd",
          "name": "getPagesPagePreview",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.onenote.com",
              "path": [
                "api",
                "v1.0",
                "me",
                "notes",
                "pages/:pageId/preview"
              ],
              "query": [
                {
                  "key": "Content-Type",
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
            "body": {
              "mode": "raw"
            },
            "description": "Returns preview text and (if there is one) a preview image for the specified page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f187a6bc-eaab-4866-8cf4-ca01676a79cb"
            }
          ]
        }
      ]
    }
  ]
}