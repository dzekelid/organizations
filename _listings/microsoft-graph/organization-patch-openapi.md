---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Update Organization
  description: Update organization Update the properties of the currently authenticated
    organization.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organization:
    get:
      summary: Get Organization
      description: Get organization Retrieve the properties and relationships of currently
        authenticated organization.
      operationId: GetOrganization
      x-api-path-slug: organization-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - Organization
    patch:
      summary: Update Organization
      description: Update organization Update the properties of the currently authenticated
        organization.
      operationId: UpdateOrganization
      x-api-path-slug: organization-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - Organization
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