{
  "info": {
    "name": "Open FinTech List of organizations",
    "_postman_id": "81084d31-b27f-40d6-b461-a7694e540b20",
    "description": "This endpoint retrievs the list of organizations present in the system. The data displays general, public information, without reference to the type of activity (for example - name, address, contacts, etc.).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "bef748f4-e2f3-470e-8d16-ecc388a7a076",
          "name": "organizations.get",
          "request": {
            "url": "http://api.openfintech.io/v1/organizations?filter[industries]=%7B%7D&filter[search]=%7B%7D&No Name=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This endpoint retrievs the list of organizations present in the system. The data displays general, public information, without reference to the type of activity (for example - name, address, contacts, etc.)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a0b5ee1-edb1-47c5-8924-9db10310045b"
            }
          ]
        }
      ]
    }
  ]
}