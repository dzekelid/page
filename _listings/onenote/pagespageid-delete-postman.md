{
  "info": {
    "name": "One Note Delete Pages Pageid",
    "_postman_id": "ea68b697-52a1-412f-bb96-f6f9b655149f",
    "description": "Deletes the specified page.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pages",
      "item": [
        {
          "id": "b9ec8287-5283-4b51-a2ae-9f5ff02f82e3",
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
              "id": "60f23240-d8bf-41d3-a634-1956081e8293"
            }
          ]
        }
      ]
    }
  ]
}