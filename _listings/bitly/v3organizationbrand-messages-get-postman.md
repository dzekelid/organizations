{
  "info": {
    "name": "Bitly Organization Metric API Organization Brand Messages",
    "_postman_id": "c6926244-8fb3-4504-86d2-9bdc74a2729d",
    "description": "Returns the top Bitlinks created by you with traffic, that did not also have non-organization traffic in the same time period, ordered by clicks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organization",
      "item": [
        {
          "id": "80b4a2f6-5500-43a5-a037-96248e045b67",
          "name": "organizationBrandMessages",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/brand_messages?domain=%7B%7D&limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top Bitlinks created by you with traffic, that did not also have non-organization traffic in the same time period, ordered by clicks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6580d48-c843-4264-a52a-fca2f6bb25b7"
            }
          ]
        }
      ]
    }
  ]
}