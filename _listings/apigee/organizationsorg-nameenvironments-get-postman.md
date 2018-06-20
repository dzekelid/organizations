{
  "info": {
    "name": "Apigee Edge Get Organizations Name Environments",
    "_postman_id": "4af8939d-bf84-46af-abc2-a4da338f18c8",
    "description": "Lists all the environments in an organization.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "5939c225-0d73-4664-b157-ac13746f8f12",
          "name": "getOrganizationsOrgNameEnvironments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.enterprise.apigee.com",
              "path": [
                "v1",
                "organizations/:org_name/environments"
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
            "description": "Lists all the environments in an organization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0259870a-87c5-4043-8592-886b03bcece4"
            }
          ]
        }
      ]
    }
  ]
}