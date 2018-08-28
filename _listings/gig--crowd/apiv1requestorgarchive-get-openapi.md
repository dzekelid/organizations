---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Request Org Archive
  version: 1.0.0
  description: Get request org archive.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/account/register/org:
    post:
      summary: Post Account Register Org
      description: Post account register org.
      operationId: postApiV1AccountRegisterOrg
      x-api-path-slug: apiv1accountregisterorg-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Org
  /api/v1/org/{userId}:
    get:
      summary: Get Org Userid
      description: Get org userid.
      operationId: getApiV1OrgUser
      x-api-path-slug: apiv1orguserid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Org
      - Userid
    post:
      summary: Post Org Userid
      description: Post org userid.
      operationId: postApiV1OrgUser
      x-api-path-slug: apiv1orguserid-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Org
      - Userid
  /api/v1/request/org/invite:
    post:
      summary: Post Request Org Invite
      description: Post request org invite.
      operationId: postApiV1RequestOrgInvite
      x-api-path-slug: apiv1requestorginvite-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Org
      - Invite
  /api/v1/request/org/out:
    get:
      summary: Get Request Org Out
      description: Get request org out.
      operationId: getApiV1RequestOrgOut
      x-api-path-slug: apiv1requestorgout-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Request
      - Org
      - Out
  /api/v1/request/org/archive:
    get:
      summary: Get Request Org Archive
      description: Get request org archive.
      operationId: getApiV1RequestOrgArchive
      x-api-path-slug: apiv1requestorgarchive-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Request
      - Org
      - Archive
  /api/v1/request/org/reject:
    post:
      summary: Post Request Org Reject
      description: Post request org reject.
      operationId: postApiV1RequestOrgReject
      x-api-path-slug: apiv1requestorgreject-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Org
      - Reject
  /api/v1/request/org/accept:
    post:
      summary: Post Request Org Accept
      description: Post request org accept.
      operationId: postApiV1RequestOrgAccept
      x-api-path-slug: apiv1requestorgaccept-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Request
      - Org
      - Accept
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