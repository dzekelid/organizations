swagger: "2.0"
x-collection-name: Xero
x-complete: 1
info:
  title: Xero oAuth 1a
  description: a-collection-to-authenticate-to-the-xero-api-using-oauth1-0a
  version: 1.0.0
host: api.xero.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Organisation:
    get:
      summary: Get Organisation
      description: Get organisation.
      operationId: getOrganisation
      x-api-path-slug: organisation-get
      responses:
        200:
          description: OK
      tags:
      - Organisation
    x-related-model:
      summary: X-related-model Organisation
      description: X-related-model organisation.
      operationId: x-related-modelOrganisation
      x-api-path-slug: organisation-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Organisation
  /Organisation/{ShortCode}:
    get:
      summary: Get Organisation Shortcode
      description: Get organisation shortcode.
      operationId: getOrganisationShortcode
      x-api-path-slug: organisationshortcode-get
      parameters:
      - in: path
        name: ShortCode
      responses:
        200:
          description: OK
      tags:
      - Organisation
      - ShortCode
    x-related-model:
      summary: X-related-model Organisation Shortcode
      description: X-related-model organisation shortcode.
      operationId: x-related-modelOrganisationShortcode
      x-api-path-slug: organisationshortcode-xrelatedmodel
      responses:
        200:
          description: OK
      tags:
      - Organisation
      - ShortCode
  /api.xro/2.0/Organisation:
    get:
      summary: Organisation
      description: 'TODO: Add Description'
      operationId: ApiXro20OrganisationGet
      x-api-path-slug: api-xro2-0organisation-get
      parameters:
      - in: header
        name: accept
      responses:
        200:
          description: OK
      tags:
      - ""