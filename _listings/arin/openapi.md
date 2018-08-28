swagger: "2.0"
x-collection-name: ARIN
x-complete: 1
info:
  title: Reverse DNS API
  description: for-managing-reverse-dns-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: www.arin.net
basePath: /regrws/core/v1
paths:
  /orgs:
    get:
      summary: Manages organizations
      description: ""
      operationId: organizations
      x-api-path-slug: orgs-get
      parameters:
      - in: query
        name: dba
        description: the name the organization does business as
        type: string
        format: string
      - in: query
        name: handle
        description: the handle of the organization
        type: string
        format: string
      - in: query
        name: name
        description: the name of organization
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /poc/org:
    get:
      summary: Organizations
      description: lists the organizations associated with a given POC.
      operationId: pocOrg
      x-api-path-slug: pocorg-get
      responses:
        200:
          description: OK
      tags:
      - Organizations