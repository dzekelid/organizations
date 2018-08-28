---
swagger: "2.0"
x-collection-name: Google Cloud Resource Manager
x-complete: 0
info:
  title: Google Cloud Resource Manager API TEst Organization IAM Permissions
  description: |-
    Returns permissions that a caller has on the specified Organization.
    The `resource` field should be the organization's resource name,
    e.g. "organizations/123".
  contact:
    name: Google
    url: https://google.com
  version: v1
host: cloudresourcemanager.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/organizations:search:
    post:
      summary: Search Organization
      description: |-
        Searches Organization resources that are visible to the user and satisfy
        the specified filter. This method returns Organizations in an unspecified
        order. New Organizations do not necessarily appear at the end of the
        results.
      operationId: cloudresourcemanager.organizations.search
      x-api-path-slug: v1organizationssearch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organization
  /v1/{resource}:getIamPolicy:
    post:
      summary: Get Organization IAM Policy
      description: |-
        Gets the access control policy for an Organization resource. May be empty
        if no such policy or resource exists. The `resource` field should be the
        organization's resource name, e.g. "organizations/123".
      operationId: cloudresourcemanager.organizations.getIamPolicy
      x-api-path-slug: v1resourcegetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being requested'
      responses:
        200:
          description: OK
      tags:
      - Organization
  /v1/{resource}:setIamPolicy:
    post:
      summary: Set Organization IAM Policy
      description: |-
        Sets the access control policy on an Organization resource. Replaces any
        existing policy. The `resource` field should be the organization's resource
        name, e.g. "organizations/123".
      operationId: cloudresourcemanager.organizations.setIamPolicy
      x-api-path-slug: v1resourcesetiampolicy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy is being specified'
      responses:
        200:
          description: OK
      tags:
      - Organization
  /v1/{resource}:testIamPermissions:
    post:
      summary: TEst Organization IAM Permissions
      description: |-
        Returns permissions that a caller has on the specified Organization.
        The `resource` field should be the organization's resource name,
        e.g. "organizations/123".
      operationId: cloudresourcemanager.organizations.testIamPermissions
      x-api-path-slug: v1resourcetestiampermissions-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resource
        description: 'REQUIRED: The resource for which the policy detail is being
          requested'
      responses:
        200:
          description: OK
      tags:
      - Organization
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