{
  "info": {
    "name": "Donors Choose Get Giving Page",
    "_postman_id": "1a31f67c-4b80-4982-9359-2451f78ea9a3",
    "description": "Get Giving Page",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Generate",
      "item": [
        {
          "id": "d2e6e47c-0325-4865-b881-6bdb15d98dbb",
          "name": "generate-gift-code",
          "request": {
            "url": "http://api.donorschoose.org/common/json_api.html",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Generate Gift Code"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ae75312-34eb-48d0-9566-f7b035ee5107"
            }
          ]
        }
      ]
    },
    {
      "name": "Giving",
      "item": [
        {
          "id": "43fd789c-a352-44dc-b2a2-493bbc411df1",
          "name": "get-giving-page",
          "request": {
            "url": "http://api.donorschoose.org/common/json_challenge.html",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Giving Page"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "654651b7-2735-40cb-8ee4-980446a8b185"
            }
          ]
        }
      ]
    }
  ]
}