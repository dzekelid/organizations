swagger: "2.0"
x-collection-name: Google Cloud Resource Manager
x-complete: 1
info:
  title: Google Cloud Resource Manager
  description: the-google-cloud-resource-manager-api-provides-methods-for-creating-reading-and-updating-project-metadata-
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