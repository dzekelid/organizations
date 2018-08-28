{
  "info": {
    "name": "Learnifier Get Organization Unit with External Id",
    "_postman_id": "6ca1144f-172d-4e62-8b24-3fb819c4dc7c",
    "description": "Returns information about the organization unit with the specified external id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "88964489-b313-4db7-803f-a228426023cf",
          "name": "extorgunit.get",
          "request": {
            "url": "http://learnifier.com/extorgunit?extid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the organization unit with the specified external id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cecca6d0-cfc6-4a5b-9740-6e4529c9052c"
            }
          ]
        }
      ]
    }
  ]
}