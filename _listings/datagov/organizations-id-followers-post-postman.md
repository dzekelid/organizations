{
  "info": {
    "name": "Data.gov API Add Organizations  Followers",
    "_postman_id": "0948ba69-d4de-4256-a185-a0154f769c05",
    "description": "Follow an object given its ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "147014d8-ad04-4fca-93e2-e20584ba205f",
          "name": "postOrganizationsFollowers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "organizations/:id/followers/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Follow an object given its ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b7c728b-252f-4133-91fe-7336d9cc9f74"
            }
          ]
        }
      ]
    }
  ]
}