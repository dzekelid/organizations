{
  "info": {
    "name": "Clarity Accounting Get Organisation Shortcode",
    "_postman_id": "3b6c013a-31cf-40f8-98d4-642b1a5be14c",
    "description": "Get organisation shortcode.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organisation",
      "item": [
        {
          "id": "0d8a4305-094d-4d46-b80e-ee2d21fc679a",
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
              "id": "5394aaab-345b-47f1-b995-0332c30985fe"
            }
          ]
        }
      ]
    }
  ]
}