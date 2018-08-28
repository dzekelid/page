{
  "info": {
    "name": "One Note Get Pages Pageid",
    "_postman_id": "40f1fb40-668f-4c06-8113-9eaa8ac0240e",
    "description": "Returns the specified page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pages",
      "item": [
        {
          "id": "0149076b-3fcb-4331-9f28-73508bc62787",
          "name": "getPagesPage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.onenote.com",
              "path": [
                "api",
                "v1.0",
                "me",
                "notes",
                "pages/:pageId"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pagelevel",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "select",
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
            "description": "Returns the specified page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "474128c0-26fe-44a7-89d2-7e9982dcc984"
            }
          ]
        },
        {
          "id": "39fa2d2e-ad51-4bfe-afc2-13d6646e9d35",
          "name": "deletePagesPage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.onenote.com",
              "path": [
                "api",
                "v1.0",
                "me",
                "notes",
                "pages/:pageId"
              ],
              "variable": [
                {
                  "id": "pageId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified page."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93ba17c1-99e8-4b80-9ea6-30e595864400"
            }
          ]
        }
      ]
    }
  ]
}