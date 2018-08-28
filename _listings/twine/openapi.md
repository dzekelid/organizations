swagger: "2.0"
x-collection-name: Twine
x-complete: 1
info:
  title: Twine
  description: -overviewthe-twine-health-api-is-restful-api--the-requests-and-responses-are-formated-according-to-the-json-apihttpjsonapi-orgformat1-0-specification-in-addition-to-this-documentation-we-also-provide-an-openapihttpsgithub-comoaiopenapispecificationblobmasterversions2-0-md-yaml-file-describing-the-api-twine-api-specificationswagger-yaml--authenticationauthentication-for-the-twine-api-is-based-on-the-oauth-2-0-authorization-frameworkhttpstools-ietf-orghtmlrfc6749--twine-currently-supports-grant-types-of-client-credentials-and-refresh-token-see-post-oauthtokenoperationcreatetoken-for-details-on-the-request-and-response-formats--redocinject-securitydefinitions-
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organization/{id}:
    get:
      summary: Get an organization
      description: Get an organization record by id.
      operationId: fetchOrganization
      x-api-path-slug: organizationid-get
      parameters:
      - in: path
        name: id
        description: Organization identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Organization
  /oauth/token/{id}/organization:
    get:
      summary: Get the organization for a token
      description: Get the organization a token can be used to access.
      operationId: fetchTokenOrganization
      x-api-path-slug: oauthtokenidorganization-get
      parameters:
      - in: path
        name: id
        description: Token identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Organizationa
      - Token