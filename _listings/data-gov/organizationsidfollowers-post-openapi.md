---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Organizations  Followers
  description: Follow an object given its ID
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/:
    get:
      summary: Get Organizations
      description: List or search all organizations
      operationId: getOrganizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: datasets
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: followers
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: permitted_reuses
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      responses:
        200:
          description: OK
      tags:
      - Organizations
    post:
      summary: Add Organizations
      description: Create a new organization
      operationId: postOrganizations
      x-api-path-slug: organizations-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/badges/:
    get:
      summary: Get Organizations Badges
      description: List all available organization badges and their labels
      operationId: getOrganizationsBadges
      x-api-path-slug: organizationsbadges-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Badges
  /organizations/suggest/:
    get:
      summary: Get Organizations Suggest
      description: Suggest organizations
      operationId: getOrganizationsSuggest
      x-api-path-slug: organizationssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Suggest
  /organizations/{id}/followers/:
    delete:
      summary: Delete Organizations  Followers
      description: Unfollow an object given its ID
      operationId: deleteOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
    get:
      summary: Get Organizations  Followers
      description: List all followers for a given object
      operationId: getOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
    post:
      summary: Add Organizations  Followers
      description: Follow an object given its ID
      operationId: postOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
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