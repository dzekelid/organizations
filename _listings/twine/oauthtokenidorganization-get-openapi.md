---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Get the organization for a token
  description: Get the organization a token can be used to access.
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organization/{id}:
    get:
      summary: Get an organization
      description: Get an organization record by id.
      operationId: fetchOrganization
      x-api-path-slug: organizationid-get
      parameters:
      - in: path
        name: id
        description: Organization identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Organization
  /oauth/token/{id}/organization:
    get:
      summary: Get the organization for a token
      description: Get the organization a token can be used to access.
      operationId: fetchTokenOrganization
      x-api-path-slug: oauthtokenidorganization-get
      parameters:
      - in: path
        name: id
        description: Token identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Organizationa
      - Token
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---