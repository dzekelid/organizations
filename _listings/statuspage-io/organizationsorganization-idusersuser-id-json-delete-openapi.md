---
swagger: "2.0"
x-collection-name: StatusPage.io
x-complete: 0
info:
  title: StatusPage.io Delete a user
  version: 1.0.0
  description: Delete a user
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
    post:
      summary: Create a user
      description: Create a user
      operationId: create-a-user
      x-api-path-slug: organizationsorganization-idusers-json-post
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/[organization_id]/users/[user_id].json:
    delete:
      summary: Delete a user
      description: Delete a user
      operationId: delete-a-user
      x-api-path-slug: organizationsorganization-idusersuser-id-json-delete
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