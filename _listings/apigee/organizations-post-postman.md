{
  "info": {
    "name": "Apigee Edge Post Organizations",
    "_postman_id": "de5596e8-8a1c-4721-afc6-a819925360c6",
    "description": "Creates an organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "20005525-f1c9-4114-8ffb-69e14f3a2147",
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
              "id": "23250945-0a6e-4295-b02a-bce335017e89"
            }
          ]
        },
        {
          "id": "eb8d0ead-fad5-4511-9339-ea3de9b52e0c",
          "name": "postOrganizations",
          "request": {
            "url": "http://api.enterprise.apigee.com/v1/organizations?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5e2a324-1ace-47c5-9ac1-f395ac7a1bc0"
            }
          ]
        }
      ]
    }
  ]
}