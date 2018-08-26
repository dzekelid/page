{
  "info": {
    "name": "Dezrez Gets a paged amount of offerss.",
    "_postman_id": "62ad80ad-e705-432a-8758-0d051591735f",
    "description": "Gets a paged amount of offerss..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Record",
      "item": [
        {
          "id": "f197565f-ab17-4040-ad82-6497ae75e0b8",
          "name": "Stats_RecordVisitBypageTypeByentityIdByroleId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/stats/RecordVisit/:pageType/:entityId"
              ],
              "query": [
                {
                  "key": "roleId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "entityId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "pageType",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Record and timestamp a visit to a 'page' on rezi.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67235491-e058-40ec-a57e-828f0abd78c1"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "8ba20c20-a5dd-4a46-94e9-0bb21a63c681",
          "name": "Offer_GetBypageSizeBypageNumber",
          "request": {
            "url": "http://api.dezrez.com/api/Offer?pageNumber=%7B%7D&pageSize=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a paged amount of offerss.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d104a21-94dc-429c-8ab4-44f55e113a7a"
            }
          ]
        }
      ]
    }
  ]
}