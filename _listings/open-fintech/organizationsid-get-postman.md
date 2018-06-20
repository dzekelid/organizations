{
  "info": {
    "name": "Open FinTech Organization by ID",
    "_postman_id": "8f1b29ed-0ac0-41ba-b16f-6377576db7ff",
    "description": "Returns organization with specific ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organizations",
      "item": [
        {
          "id": "748b5ef7-0a2e-4082-bb68-8a1a49af80dc",
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
              "id": "c6999cad-1d31-40e2-9026-e1233b3b1abf"
            }
          ]
        },
        {
          "id": "f2a3ad75-9744-402f-a549-09ded1db4559",
          "name": "organizations.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.openfintech.io",
              "path": [
                "v1",
                "organizations/:id"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns organization with specific ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "75eb4af9-cbab-4b56-9480-5130d61a35bd"
            }
          ]
        }
      ]
    }
  ]
}