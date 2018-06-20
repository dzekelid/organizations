{
  "info": {
    "name": "Data.gov API Delete Organizations  Followers",
    "_postman_id": "cf6c91dd-2feb-4bc3-8e28-010cbd61f6af",
    "description": "Unfollow an object given its ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "596e5979-7fdd-4033-ba6e-9f93d8f8a23d",
          "name": "deleteOrganizationsFollowers",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unfollow an object given its ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d81a5d9e-341d-4a3e-a57d-deaf3726dd8a"
            }
          ]
        }
      ]
    }
  ]
}