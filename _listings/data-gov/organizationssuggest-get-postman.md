{
  "info": {
    "name": "Data.gov API Get Organizations Suggest",
    "_postman_id": "eff6e8e5-7ffe-4699-8cf0-e3c0d4822fbc",
    "description": "Suggest organizations",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "e4b49fe1-7fc3-4cba-a3e2-1bbc8345db6c",
          "name": "getOrganizationsSuggest",
          "request": {
            "url": "http://catalog.data.gov/api/3/organizations/suggest/?q=%7B%7D&size=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Suggest organizations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e8bf17b-2e75-4483-8c35-33fa5bef5ead"
            }
          ]
        }
      ]
    }
  ]
}