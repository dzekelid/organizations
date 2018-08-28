{
  "info": {
    "name": "Data.gov API Get Me Org Issues",
    "_postman_id": "7c69d55e-c686-48d7-862e-12c1197ab284",
    "description": "List all issues related to my organizations",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "me",
      "item": [
        {
          "id": "8d92cb1f-2e0b-4c7c-b530-0f42fbdff055",
          "name": "getMeOrgIssues",
          "request": {
            "url": "http://catalog.data.gov/api/3/me/org_issues/?q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all issues related to my organizations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c59ce75a-df8d-4f6a-86dd-fed2918bcee9"
            }
          ]
        }
      ]
    }
  ]
}