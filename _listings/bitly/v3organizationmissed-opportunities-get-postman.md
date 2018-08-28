{
  "info": {
    "name": "Bitly Organization Metric API Organization Missed Opportunities",
    "_postman_id": "e46f5742-384e-4c08-a9af-34f32851b7ed",
    "description": "Returns the top links shared by your audience, but not by you, ordered by clicks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Organization",
      "item": [
        {
          "id": "f668fbb4-733b-4778-b06a-48d03315440c",
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
              "id": "505893a4-3208-447c-81b1-ef1cb95993c1"
            }
          ]
        },
        {
          "id": "52f38ebb-f53a-490b-96af-adf9a6472d64",
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
              "id": "5fdd4745-e0d5-4855-91d3-6a5b75ab06ae"
            }
          ]
        },
        {
          "id": "6672a877-2903-4956-b51c-5f06165043d2",
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
              "id": "9c7b24c7-1bcf-40db-a6ab-b90bc4cf99d0"
            }
          ]
        },
        {
          "id": "ece761a5-087b-4006-bc2a-2704ed69c878",
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
              "id": "0b9d7d4c-3f71-4e8c-b5be-8312b429afca"
            }
          ]
        },
        {
          "id": "51052dd1-d61d-4144-8da7-1d843185a12a",
          "name": "organizationMissedOpportunities",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/v3/organization/missed_opportunities?an epoch timestamp, indicating the most recent time for which to pull metrics. default:now=%7B%7D&domain=%7B%7D&limit=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D&unit_reference_ts=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top links shared by your audience, but not by you, ordered by clicks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fe7d5027-5350-480a-8465-00d9771168bc"
            }
          ]
        }
      ]
    }
  ]
}