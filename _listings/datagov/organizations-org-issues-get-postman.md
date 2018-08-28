{
  "info": {
    "name": "Data.gov API Get Organizations Org Issues",
    "_postman_id": "fb9fa982-43c2-4cf5-96b3-6a69c69aae92",
    "description": "List organization issues",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "5dfebf63-dfab-4dd9-b680-6ee9986d51e6",
          "name": "getOrganizationsOrgIssues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "organizations/:org/issues/"
              ],
              "variable": [
                {
                  "id": "org",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List organization issues"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02d5351e-60b9-4191-8a31-b47fb704c276"
            }
          ]
        }
      ]
    }
  ]
}