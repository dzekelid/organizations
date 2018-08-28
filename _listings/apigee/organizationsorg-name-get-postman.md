{
  "info": {
    "name": "Apigee Edge Get Organizations Name",
    "_postman_id": "9be44477-8a08-4ae0-8b45-f1c324a6d976",
    "description": "Gets a specific organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "cf77b086-4126-4ad7-9c80-575347467b41",
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
              "id": "f9e6f076-4960-4091-8d38-7b438d2d7dae"
            }
          ]
        },
        {
          "id": "619f2a2b-3721-4ea8-9449-cef890e83cd8",
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
              "id": "c8197547-0ea0-499b-916f-bdd0d8470e21"
            }
          ]
        },
        {
          "id": "990871ba-5c94-4916-aedf-1517e55976aa",
          "name": "getOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name"
              ],
              "variable": [
                {
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a specific organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10baf62f-f44e-40a2-b46c-f8bbb879411e"
            }
          ]
        }
      ]
    }
  ]
}