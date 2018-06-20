---
swagger: "2.0"
x-collection-name: Gitter
x-complete: 1
info:
  title: No Title
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/:userId/orgs:
    get:
      summary: User Orgs
      description: List of the user's GitHub Organisations and their respective Room
        if available.
      operationId: getUserOrgs
      x-api-path-slug: useruseridorgs-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Organizations
---