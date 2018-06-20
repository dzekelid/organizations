---
swagger: "2.0"
x-collection-name: Envestnet
x-complete: 0
info:
  title: Crunch Base Organizations
  description: Get Organizations
  termsOfService: https://data.crunchbase.com/v3/page/accessing-the-dataset
  contact:
    name: Crunchbase
    url: https://groups.google.com/forum/#!forum/crunchbase-api
    email: data@crunchbase.com
  version: v3
host: api.crunchbase.com
basePath: /v/3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations:
    get:
      summary: Organizations
      description: Get Organizations
      operationId: organizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: categories
        description: Filter by categories (comma separated, ANDd together) e
      - in: query
        name: category_uuids
        description: Filter by one or more Categories
      - in: query
        name: domain_name
        description: Text search of an Organizations domain_name (e
      - in: query
        name: locations
        description: Filter by location names (comma separated, ANDd together) e
      - in: query
        name: name
        description: Full text search limited to name and aliases
      - in: query
        name: organization_types
        description: Filter by one or more types
      - in: query
        name: page
        description: Page number of the results to retrieve
      - in: query
        name: query
        description: Full text search of an Organizations name, aliases (i
      - in: query
        name: sort_order
        description: The sort order of the collection
      - in: query
        name: updated_since
        description: Timestamp When provided, restricts the result set to Organizations
          where updated_at >= the passed value
      - in: query
        name: user_key
        description: 'Possible values are: 7a582a92032069b4f775a15b1acbe256'
      responses:
        200:
          description: OK
      tags:
      - Organizations
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