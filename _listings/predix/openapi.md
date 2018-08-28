swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/organizations/{organization_id}:
    parameters:
      summary: Parameters Organizations
      description: Parameters organizations.
      operationId: parametersV1OrganizationsOrganization
      x-api-path-slug: v1organizationsorganization-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Organizations
    get:
      summary: Get Organizations
      description: You can retrieve an organization by GUID using the following parameters.
      operationId: getV1OrganizationsOrganization
      x-api-path-slug: v1organizationsorganization-id-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
    post:
      summary: Post Organizations
      description: You can update an organization using the following parameters.
      operationId: postV1OrganizationsOrganization
      x-api-path-slug: v1organizationsorganization-id-post
      parameters:
      - in: body
        name: body
        description: Body Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /v1/organizations/{organization_id}/subscriptions:
    parameters:
      summary: Parameters Organizations Subscriptions
      description: Parameters organizations subscriptions.
      operationId: parametersV1OrganizationsOrganizationSubscriptions
      x-api-path-slug: v1organizationsorganization-idsubscriptions-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Organizations
      - Subscriptions
    post:
      summary: Post Organizations Subscriptions
      description: Create a new subscription to a plan.
      operationId: postV1OrganizationsOrganizationSubscriptions
      x-api-path-slug: v1organizationsorganization-idsubscriptions-post
      parameters:
      - in: body
        name: body
        description: Body Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Subscriptions
  /v1/organizations/{organization_id}/subscriptions/{subscription_id}:
    parameters:
      summary: Parameters Organizations Subscriptions
      description: Parameters organizations subscriptions.
      operationId: parametersV1OrganizationsOrganizationSubscriptionsSubscription
      x-api-path-slug: v1organizationsorganization-idsubscriptionssubscription-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - Organizations
      - Subscriptions
    put:
      summary: Put Organizations Subscriptions
      description: You can update a subscription's plan, using the following parameters.
      operationId: putV1OrganizationsOrganizationSubscriptionsSubscription
      x-api-path-slug: v1organizationsorganization-idsubscriptionssubscription-id-put
      parameters:
      - in: body
        name: body
        description: Body Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Subscriptions
    delete:
      summary: Delete Organizations Subscriptions
      description: You can cancel a plan subscription using the following parameters.
        When the last subscription is canceled, the customer will become canceled.
      operationId: deleteV1OrganizationsOrganizationSubscriptionsSubscription
      x-api-path-slug: v1organizationsorganization-idsubscriptionssubscription-id-delete
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Subscriptions