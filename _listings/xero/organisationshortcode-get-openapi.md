---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Get Organisation Shortcode
  description: Get organisation shortcode.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
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