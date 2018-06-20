---
swagger: "2.0"
x-collection-name: Open FinTech
x-complete: 0
info:
  title: Open FinTech Organization by ID
  description: Returns organization with specific ID.
  version: "2017-08-24"
host: api.openfintech.io
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations:
    get:
      summary: List of organizations
      description: This endpoint retrievs the list of organizations present in the
        system. The data displays general, public information, without reference to
        the type of activity (for example - name, address, contacts, etc.).
      operationId: organizations.get
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: filter[industries]
        description: Filtering by industries
      - in: query
        name: filter[search]
        description: Full text search with id, name, code
      - in: query
        name: No Name
      - in: query
        name: sort
        description: Sort params:| ASC | DESC ||-----|------|| name | -name || code
          | -code || status | -status || description | -description |
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/{id}:
    get:
      summary: Organization by ID
      description: Returns organization with specific ID.
      operationId: organizations.id.get
      x-api-path-slug: organizationsid-get
      parameters:
      - in: query
        name: No Name
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