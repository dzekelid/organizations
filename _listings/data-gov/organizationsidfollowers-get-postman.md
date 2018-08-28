{
  "info": {
    "name": "Data.gov API Get Organizations  Followers",
    "_postman_id": "9e148604-dba9-48a8-834f-b44ec4af032d",
    "description": "List all followers for a given object",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "727c99a7-bfa9-4b42-8c39-8f2600c28fee",
          "name": "getOrganizationsFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "organizations/:id/followers/"
              ],
              "query": [
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page_size",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all followers for a given object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cd56f3b-66fc-4f58-8f1d-b17fc4a07694"
            }
          ]
        }
      ]
    }
  ]
}