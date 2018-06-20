{
  "info": {
    "name": "Data.gov API Delete Organizations Org",
    "_postman_id": "c1a88ca5-2081-4a9c-a664-129206e1738e",
    "description": "Delete a organization given its identifier",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "ac0bec8b-6c73-4b98-99dd-66d7cb61bea3",
          "name": "deleteOrganizationsOrg",
          "request": {
            "url": {
              "protocol": "http",
              "host": "catalog.data.gov",
              "path": [
                "api",
                "3",
                "organizations/:org/"
              ],
              "variable": [
                {
                  "id": "org",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a organization given its identifier"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44f09e34-b236-4604-9fea-aad30420904f"
            }
          ]
        }
      ]
    }
  ]
}