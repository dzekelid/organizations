---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Organizations
  description: Create a new organization
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/:
    get:
      summary: Get Organizations
      description: List or search all organizations
      operationId: getOrganizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: datasets
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: followers
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: permitted_reuses
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      responses:
        200:
          description: OK
      tags:
      - Organizations
    post:
      summary: Add Organizations
      description: Create a new organization
      operationId: postOrganizations
      x-api-path-slug: organizations-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
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