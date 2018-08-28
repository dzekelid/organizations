{
  "info": {
    "name": "Apigee Edge Get Organizations",
    "_postman_id": "c9169623-d41f-401d-811e-68d5741fc573",
    "description": "Lists all the organizations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "32c8e17d-cf90-48dc-97b9-93bdb9c39f8d",
          "name": "getOrganizations",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/organizations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all the organizations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ffcf387-39cc-440e-94c9-1b2462110d8d"
            }
          ]
        }
      ]
    }
  ]
}