---
swagger: "2.0"
x-collection-name: StatusPage.io
x-complete: 0
info:
  title: StatusPage.io List users
  version: 1.0.0
  description: List users
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/[organization_id]/users.json:
    get:
      summary: List users
      description: List users
      operationId: list-users
      x-api-path-slug: organizationsorganization-idusers-json-get
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