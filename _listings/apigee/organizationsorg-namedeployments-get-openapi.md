---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Get Organizations Name Deployments
  description: Gets all deployments of an organization.
  version: 1.0.0
host: api.enterprise.apigee.com
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
      summary: Get Organizations
      description: Lists all the organizations.
      operationId: getOrganizations
      x-api-path-slug: organizations-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
    post:
      summary: Post Organizations
      description: Creates an organization.
      operationId: postOrganizations
      x-api-path-slug: organizations-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/{org_name}:
    get:
      summary: Get Organizations Name
      description: Gets a specific organization.
      operationId: getOrganizationsOrgName
      x-api-path-slug: organizationsorg-name-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
    put:
      summary: Put Organizations Name
      description: Updates the description of a specific organization.
      operationId: putOrganizationsOrgName
      x-api-path-slug: organizationsorg-name-put
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
    delete:
      summary: Delete Organizations Name
      description: Deletes a specific organization.
      operationId: deleteOrganizationsOrgName
      x-api-path-slug: organizationsorg-name-delete
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/{org_name}/deployments:
    get:
      summary: Get Organizations Name Deployments
      description: Gets all deployments of an organization.
      operationId: getOrganizationsOrgNameDeployments
      x-api-path-slug: organizationsorg-namedeployments-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Deployments
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