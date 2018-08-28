{
  "info": {
    "name": "Apigee Edge Put Organizations Name",
    "_postman_id": "5423d5c5-a4be-4c5c-b087-2bdc3fcc35f6",
    "description": "Updates the description of a specific organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "68e7b7ed-ec07-4ecf-a0d1-ee41e9debd3b",
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
              "id": "4802d8f5-8258-41cc-8494-a2873fbce926"
            }
          ]
        },
        {
          "id": "a33f9d77-206a-4a7f-b4f1-0e27576c96e6",
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
              "id": "698424ed-7724-425b-9aec-fed21e1d32fd"
            }
          ]
        },
        {
          "id": "d6846281-6c55-46c6-8afb-313436ee2262",
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
              "id": "6b365bf6-5327-46a9-86ba-65c30c86f39d"
            }
          ]
        },
        {
          "id": "322c1ed5-e19d-4d22-b60b-3ae9eb5d37d9",
          "name": "putOrganizationsOrgName",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name"
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
                  "id": "org_name",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the description of a specific organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1aadb1d0-037a-418a-9174-9dbb06847e97"
            }
          ]
        }
      ]
    }
  ]
}