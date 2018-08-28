---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Create a organization
  description: Create a organization
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations:
    get:
      summary: Retrieve a list of organizations
      description: Retrieve a list of organizations
      operationId: retrieve-a-list-of-organizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Organizations
    post:
      summary: Create a organization
      description: Create a organization
      operationId: create-a-organization
      x-api-path-slug: organizations-post
      parameters:
      - in: body
        name: body
        description: Organization resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organization
  /organizations/{id}:
    delete:
      summary: Delete a organization
      description: Delete a organization with predefined identifier string
      operationId: delete-a-organization-with-predefined-identifier-string
      x-api-path-slug: organizationsid-delete
      responses:
        200:
          description: OK
      tags:
      - Organization
    get:
      summary: Retrieve a organization
      description: Retrieve a organization with specified identifier string
      operationId: retrieve-a-organization-with-specified-identifier-string
      x-api-path-slug: organizationsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Organization
    put:
      summary: Create or update a organization with predefined ID
      description: Create or update a organization with predefined identifier string
      operationId: create-or-update-a-organization-with-predefined-identifier-string
      x-api-path-slug: organizationsid-put
      parameters:
      - in: body
        name: body
        description: Organization resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - Organization
      - Predefined
      - ID
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