{
  "info": {
    "name": "Clarity Accounting X-related-model Organisation Shortcode",
    "_postman_id": "2c860e71-5834-4a47-a1e4-17ccc8dbb7d9",
    "description": "X-related-model organisation shortcode.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organisation",
      "item": [
        {
          "id": "fc018c90-2448-4ab9-8678-22e4ba0bac71",
          "name": "getOrganisationShortcode",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.xero.com",
              "path": [
                "api.xro",
                "2.0",
                "Organisation/:ShortCode"
              ],
              "variable": [
                {
                  "id": "ShortCode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get organisation shortcode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b2338b7-afac-48c3-a75f-671930fa7139"
            }
          ]
        }
      ]
    }
  ]
}