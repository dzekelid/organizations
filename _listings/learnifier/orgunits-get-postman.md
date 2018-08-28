{
  "info": {
    "name": "Learnifier Organization Units",
    "_postman_id": "8a7108a0-cf87-43a9-9aeb-723899d068bf",
    "description": "The orgunits endpoint returns information about the available organization units (orgunits).\nThe response includes the display name, internal and external id and client number.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "52e742c3-60c8-45af-b64c-9586ade89307",
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
              "id": "2ea9847e-fdf6-4366-aa8f-bf903d0684cc"
            }
          ]
        },
        {
          "id": "32ab7872-a6a2-4b79-8a0b-edd8f4bb46b1",
          "name": "orgunits.get",
          "request": {
            "url": "http://learnifier.com/orgunits",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The orgunits endpoint returns information about the available organization units (orgunits).\nThe response includes the display name, internal and external id and client number."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aa2c584f-1ebf-41b1-882e-41e6696a06c7"
            }
          ]
        }
      ]
    }
  ]
}