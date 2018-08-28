{
  "info": {
    "name": "Point of Contact (POC) API Organizations",
    "_postman_id": "c94361b1-350e-43d2-a9e9-8b2bd7b6db6f",
    "description": "lists the organizations associated with a given POC.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Point of Contact",
      "item": [
        {
          "id": "28516e01-b761-44ed-ac4d-b58468fcedb8",
          "name": "poc",
          "request": {
            "url": "http://example.com/api/poc?city=city&company=company&domain=domain&first=first&handle=handle&last=last&middle=middle",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "lists the Point of Contact (POC)"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acde86cd-0962-4d08-8b55-47d435c1d09e"
            }
          ]
        }
      ]
    },
    {
      "name": "Organizations",
      "item": [
        {
          "id": "59f44840-eb87-4d75-8c1d-a852f45b1a03",
          "name": "pocOrg",
          "request": {
            "url": "http://example.com/api/poc/org",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "lists the organizations associated with a given POC."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e0e11a4-afd3-4c18-924c-f5c3cd364149"
            }
          ]
        }
      ]
    }
  ]
}