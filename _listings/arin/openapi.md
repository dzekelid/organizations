---
swagger: "2.0"
x-collection-name: ARIN
x-complete: 1
info:
  title: Point of Contact (POC) API
  description: for-managing-point-of-contact-poc-
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
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
---