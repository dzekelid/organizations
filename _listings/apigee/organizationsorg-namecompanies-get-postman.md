{
  "info": {
    "name": "Apigee Edge Get Organizations Name Companies",
    "_postman_id": "c1b857d2-8a18-49fd-a388-61e890d0f5ab",
    "description": "Returns an expanded list of companies, displaying a full profile for each company in the organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "a08ba570-cb27-4b09-87b5-8554e5fa1dad",
          "name": "getOrganizationsOrgNameCompanies",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/companies"
              ],
              "query": [
                {
                  "key": "expand",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an expanded list of companies, displaying a full profile for each company in the organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "874697fa-94b1-4eae-b119-e293a0dc8e63"
            }
          ]
        }
      ]
    }
  ]
}