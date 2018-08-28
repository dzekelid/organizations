---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: Webex Teams Admin API Get Organization Details
  description: "Shows details for an organization, by ID.\r\n\r\nSpecify the org ID
    in the orgId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-organizations-orgId-get.html\r\n\r\nExample
    Response:\r\n``` json\r\n{\r\n  'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n
    \ 'displayName' : 'Acme, Inc.',\r\n  'created' : '2015-10-18T14:26:16+00:00'\r\n}\r\n```"
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations:
    get:
      summary: List Organizations
      description: |-
        List all organizations visible by your account.

        https://developer.webex.com/endpoint-organizations-get.html

        Example Response:
        ``` json
        {
          'items' : [ {
            'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
            'displayName' : 'Acme, Inc.',
            'created' : '2015-10-18T14:26:16+00:00'
          } ]
        }
        ```
      operationId: OrganizationsGet
      x-api-path-slug: organizations-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Organizations
  /organizations/{_organization}:
    get:
      summary: Get Organization Details
      description: "Shows details for an organization, by ID.\r\n\r\nSpecify the org
        ID in the orgId parameter in the URI.\r\n\r\nhttps://developer.webex.com/endpoint-organizations-orgId-get.html\r\n\r\nExample
        Response:\r\n``` json\r\n{\r\n  'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',\r\n
        \ 'displayName' : 'Acme, Inc.',\r\n  'created' : '2015-10-18T14:26:16+00:00'\r\n}\r\n```"
      operationId: OrganizationsByOrganizationGet
      x-api-path-slug: organizations-organization-get
      parameters:
      - in: path
        name: _organization
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - Organization
      - Details
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