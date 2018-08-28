swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/organizations:
    post:
      summary: Register organization
      description: Register an Organization with a name. The name must be unique,
        so if one registers an Organization with a name that is already in use, an
        error will occur.
      operationId: postApiV1Organizations
      x-api-path-slug: apiv1organizations-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Register
      - Organization
  /api/v1/events/:
    post:
      summary: Create an Event
      description: |-
        Used to create an event for a container at a specific location and time.
        Each event is defined by a type.
        Currently a limited number of events (pickup and availability) are supported, but this may be extended with e.g. passage events.
        There are 2 ways to refer to a Container: by means of its id as defined in the Blockchain (this requires recording these ids in your app), or by means of a combination of the blNumber and isoNumber. Similarly, locations can be specified in 2 ways: by means of their id as defined in the Blockchain or by means of their name. In the latter case the name must be defined in a mapping   file for the Organization you - as a user- belong to. Also note that the container may not yet be known in the Blockchain at the time
        an availability event is created!
      operationId: postApiV1Events
      x-api-path-slug: apiv1events-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Event
  /api/v1/pickup_rights/:
    get:
      summary: List PickupRights
      description: Get all PickupRights that are assigned / transferred to the users's
        Organization.
      operationId: getApiV1PickupRights
      x-api-path-slug: apiv1pickup-rights-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
      - PickupRights
  /api/v1/pickup_rights/{id}/revoke_transfer:
    put:
      summary: Revoke Transfer
      description: Revoke the current PickupRight transfer. This must be used in case
        you did a transfer of a PickupRight to another Organization and you want to
        cancel this. This action is only possible as long as the PickupRight is not
        assigned.
      operationId: putApiV1PickupRightsRevokeTransfer
      x-api-path-slug: apiv1pickup-rightsidrevoke-transfer-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: id of the PickupRight as reported by List PickupRights
      responses:
        200:
          description: OK
      tags:
      - Revoke
      - Transfer
  /api/v1/pickup_rights/{id}/transfer:
    put:
      summary: Transfer
      description: Transfer the PickupRight to another Organization (a subcontractor).
      operationId: putApiV1PickupRightsTransfer
      x-api-path-slug: apiv1pickup-rightsidtransfer-put
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: id of the PickupRight (as reported by List PickupRights)
      responses:
        200:
          description: OK
      tags:
      - Transfer
  /api/v1/releases/{id}:
    delete:
      summary: Block
      description: |-
        Blocking a release is done by a delete. This will revoke the PickupRight from the consignee. The Container and its PickupRight are deleted. Afterwards it is still possible to release again.
         The following conditions apply for this to work:
        * the container must have been released, i.e. there must be a vallid PickupRight   for the Container
        * the PickupRight should not be transferred to another Organization than the one that got the relesase initially
        * the PickupRight should not yet be assigned (to a driver / skipper)
      operationId: deleteApiV1Releases
      x-api-path-slug: apiv1releasesid-delete
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: original id of the release as defined in the client system and
          passed during the creation
      responses:
        200:
          description: OK
      tags:
      - Block