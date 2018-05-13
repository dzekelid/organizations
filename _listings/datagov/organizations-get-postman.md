{
  "info": {
    "name": "Data.gov API Get Organizations",
    "_postman_id": "6a1b8cbe-c1cf-44a8-9568-dc81c0d6bd26",
    "description": "List or search all organizations",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "organizations",
      "item": [
        {
          "id": "a7cf70d8-9fae-45fb-9d63-a3c60350916b",
          "name": "getOrganizations",
          "request": {
            "url": "http://catalog.data.gov/api/3/organizations/?badge=%7B%7D&datasets=%7B%7D&facets=%7B%7D&followers=%7B%7D&page=%7B%7D&page_size=%7B%7D&permitted_reuses=%7B%7D&q=%7B%7D&reuses=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List or search all organizations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a94b716-d3c1-4644-9648-7d7c879a287c"
            }
          ]
        }
      ]
    }
  ]
}