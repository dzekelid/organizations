swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
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