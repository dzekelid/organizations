{
  "info": {
    "name": "Bitly Organization Metric API Organization Leaderboard",
    "_postman_id": "b5c755cf-38d4-4d8f-b0f1-e3cbc1bdca73",
    "description": "Returns the top-performing organization members ordered by clicks or shortens.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organization",
      "item": [
        {
          "id": "1be412c9-8f35-4adc-8092-ae910813bf5a",
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
              "id": "47c11611-1e23-4e2a-9b83-eef055fcda14"
            }
          ]
        },
        {
          "id": "d9f2bcdf-47ec-4c0e-8fd8-e3488286c76f",
          "name": "organizationClicks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/clicks?domain=%7B%7D&limit=%7B%7D&login=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the number of clicks on Bitlinks created by your organization or by other Bitly users that point to your domains."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef052140-dab9-4b8c-b8a2-5ae9c240783f"
            }
          ]
        },
        {
          "id": "c3fffef5-e4d2-4306-8c83-3c755f3234d5",
          "name": "organizationIntersectingLinks",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/intersecting_links?domain=%7B%7D&limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top links shared by both your audience and by your account, ordered by clicks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23777ffd-d4d5-4ef2-9feb-14bf803e6839"
            }
          ]
        },
        {
          "id": "a0e73d27-45e9-4845-9ff8-19cf0a56cdac",
          "name": "organizationLeaderBoard",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/leaderboard?domain=%7B%7D&limit=%7B%7D&orderby=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top-performing organization members ordered by clicks or shortens."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69860a1f-db27-484c-a966-432b2308a3d6"
            }
          ]
        }
      ]
    }
  ]
}