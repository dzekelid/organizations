{
  "info": {
    "name": "Data.gov API Get Me Org Datasets",
    "_postman_id": "f85c3653-9c0f-4844-b96c-f49cacde1063",
    "description": "List all datasets related to me and my organizations",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "me",
      "item": [
        {
          "id": "0602c03c-0dcc-4b27-a7e9-d095e025cfc8",
          "name": "getMeOrgDatasets",
          "request": {
            "url": "http://catalog.data.gov/api/3/me/org_datasets/?q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all datasets related to me and my organizations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ab96197-31f1-46ff-874b-94bbfbd8dda3"
            }
          ]
        }
      ]
    }
  ]
}