---
swagger: "2.0"
x-collection-name: StatusPage
x-complete: 1
info:
  title: StatusPage.io
  version: 1.0.0
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
---