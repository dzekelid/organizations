---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Retrieves your own organization
  description: Retrieves the information of the login user's own organization.
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/visible:
    get:
      summary: Retrieves organizations available for collaboration
      description: "Retrieves organizations in a specific business role that are available
        for collaboration.  \nThese organizations may have been approved for or blocked
        from collaboration, or they're still pending for approval.\nThe login user
        must be from a customer."
      operationId: retrieves-organizations-in-a-specific-business-role-that-are-available-for-collaboration--these-orga
      x-api-path-slug: organizationsvisible-get
      parameters:
      - in: query
        name: activeServices
        description: The types of service that a supplier provides
      - in: query
        name: approved
        description: Specify approved=true to restrict the search to organizations
          that are approved for collaboration
      - in: query
        name: roleCode
        description: The code for the business role of the organizations
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Organizations
      - Availablecollaboration
  /organizations/self:
    get:
      summary: Retrieves your own organization
      description: Retrieves the information of the login user's own organization.
      operationId: retrieves-the-information-of-the-login-users-own-organization
      x-api-path-slug: organizationsself-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Your
      - Own
      - Organization
  /organizations/{organizationId}:
    get:
      summary: Retrieves an organization
      description: Retrieves an organization by its ID.
      operationId: retrieves-an-organization-by-its-id
      x-api-path-slug: organizationsorganizationid-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Organization
  /organizations/{organizationId}/collaborationRooms:
    get:
      summary: Retrieves the collaboration rooms of an organization
      description: "Retrieves the collaboration rooms where the login user's organization
        is a collaboration party.   \n- If the login user is not an organization admin,
        only the collaboration rooms where the login user is a participant are retrieved.
        \  \n- If the login user is an organization admin, all the collaboration rooms
        where the login user's organization is a collaboration party are retrieved.
        The login user may not be part of the collaborations."
      operationId: retrieves-the-collaboration-rooms-where-the-login-users-organization-is-a-collaboration-party----if-
      x-api-path-slug: organizationsorganizationidcollaborationrooms-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      - in: query
        name: organizationIds
        description: The IDs of other organizations
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Rooms
      - Of
      - Organization
  /organizations/{organizationId}/collaborationRooms/owned:
    get:
      summary: Retrieves the collaboration rooms created by an organization
      description: "Retrieves the collaboration rooms created and owned by an organization.
        \ \n- If the login user is not an organization admin, only the collaboration
        rooms where the login user is a participant are retrieved.  \n- If the login
        user is an organization admin, all the collaboration rooms owned by the login
        user's organization are retrieved."
      operationId: retrieves-the-collaboration-rooms-created-and-owned-by-an-organization---if-the-login-user-is-not-an
      x-api-path-slug: organizationsorganizationidcollaborationroomsowned-get
      parameters:
      - in: path
        name: organizationId
        description: The ID of the login users organization
      - in: query
        name: organizationIds
        description: The IDs of other organizations
      - in: query
        name: partId
        description: The ID of a part
      - in: query
        name: serviceType
        description: The type of service that a supplier organization provides during
          the collaboration
      - in: query
        name: status
        description: The status of a collaboration
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Collaboration
      - Rooms
      - Created
      - By
      - Organization
  /users:
    get:
      summary: Retrieves the users of an organization
      description: "Retrieves the users of a specific organization.  \nThe login user
        must be from this organization as well."
      operationId: retrieves-the-users-of-a-specific-organization--the-login-user-must-be-from-this-organization-as-wel
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: organizationId
        description: The ID of an organization
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Users
      - Of
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