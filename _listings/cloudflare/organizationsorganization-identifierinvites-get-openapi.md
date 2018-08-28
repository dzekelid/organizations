---
swagger: "2.0"
x-collection-name: CloudFlare
x-complete: 0
info:
  title: CloudFlare List all invitations associated with an organization
  version: 1.0.0
  description: List all invitations associated with an organization
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/:identifier:
    get:
      summary: Get information about a specific organization that you are a member
        of
      description: Get information about a specific organization that you are a member
        of
      operationId: cloudflare-organizations-api
      x-api-path-slug: organizationsidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
    patch:
      summary: Update an existing Organization
      description: Update an existing Organization
      operationId: cloudflare-organizations-api
      x-api-path-slug: organizationsidentifier-patch
      parameters:
      - in: query
        name: name
        description: Organization NamettttttttttttttCloudFlare, Inc
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/:organization_id/firewall/access_rules/rules:
    get:
      summary: Search, sort, and filter IP/country access rules
      description: Search, sort, and filter IP/country access rules
      operationId: cloudflare-organizationlevel-firewall-access-rule-api
      x-api-path-slug: organizationsorganization-idfirewallaccess-rulesrules-get
      parameters:
      - in: query
        name: configuration_target
        description: The rule configuration targetttttttttttttttip
      - in: query
        name: configuration_value
        description: Search by IP, range, or country codetttttttttttttt1
      - in: query
        name: direction
        description: Direction to order rulesttttttttttttttdesc
      - in: query
        name: match
        description: Whether to match all search requirements or at least one (any)ttttttttttttttall
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: order
        description: Field to order rules byttttttttttttttmode
      - in: query
        name: page
        description: Page number of paginated resultstttttttttttttt1
      - in: query
        name: per_page
        description: Number of rules per pagetttttttttttttt50
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Firewall Access Rules
    post:
      summary: Make a new IP, IP range, or country access rule for all zones owned
        by the organization
      description: Make a new IP, IP range, or country access rule for all zones owned
        by the organization
      operationId: cloudflare-organizationlevel-firewall-access-rule-api
      x-api-path-slug: organizationsorganization-idfirewallaccess-rulesrules-post
      parameters:
      - in: query
        name: configuration
        description: Rule configurationtttttttttttttttttttttOne of the following:tttttttttttttttttttttttttttttShow
          definition &raquo;ttttttttttttttttttttttttttttttttttttttName /typetttttttttttDescription
          /exampletttttttttttConstraintstttttttttttttttttttttttttttttttttttttttttttttttttttttttttargettttttttttttttstring
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: value
        description: The IP address to target in requeststtttttttttttttttttttttttttttttttttt1
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Firewall Access Rules
  /organizations/:organization_id/firewall/access_rules/rules/:identifier:
    delete:
      summary: Remove an access rule so it is no longer evaluated during requests
      description: Remove an access rule so it is no longer evaluated during requests
      operationId: cloudflare-organizationlevel-firewall-access-rule-api
      x-api-path-slug: organizationsorganization-idfirewallaccess-rulesrulesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Organization Firewall Access Rules
    patch:
      summary: Update rule state and/or configuration
      description: Update rule state and/or configuration
      operationId: cloudflare-organizationlevel-firewall-access-rule-api
      x-api-path-slug: organizationsorganization-idfirewallaccess-rulesrulesidentifier-patch
      parameters:
      - in: query
        name: configuration
        description: Rule configurationtttttttttttttttttttttOne of the following:tttttttttttttttttttttttttttttShow
          definition &raquo;ttttttttttttttttttttttttttttttttttttttName /typetttttttttttDescription
          /exampletttttttttttConstraintstttttttttttttttttttttttttttttttttttttttttttttttttttttttttargettttttttttttttstring
      - in: query
        name: mode
        description: The action to apply to a matched requestttttttttttttttchallenge
      - in: query
        name: value
        description: The IP address to target in requeststtttttttttttttttttttttttttttttttttt1
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Firewall Access Rules
  /organizations/:organization_identifier/invite/:identifier:
    patch:
      summary: Change the Roles of a Pending Invite
      description: Change the Roles of a Pending Invite
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinviteidentifier-patch
      parameters:
      - in: query
        name: roles
        description: Array of Roles associated with the invited usertttttttttttttt[3536bcfad5faccb999b47003c79917fb]
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
  /organizations/:organization_identifier/invites:
    get:
      summary: List all invitations associated with an organization
      description: List all invitations associated with an organization
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinvites-get
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
    post:
      summary: Invite a User to become a Member of an Organization
      description: Invite a User to become a Member of an Organization
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinvites-post
      parameters:
      - in: query
        name: invited_member_email
        description: Email address of the user to be added to the Organizationttttttttttttttuser@example
      - in: query
        name: roles
        description: Array of Roles associated with the invited usertttttttttttttt[{id:5a7805061c76ada191ed06f989cc3dac},{id:9a7806061c88ada191ed06f989cc3dac}]
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
  /organizations/:organization_identifier/invites/:identifier:
    delete:
      summary: Cancel an existing invitation
      description: Cancel an existing invitation
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinvitesidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
    get:
      summary: Get the details of an invitation
      description: Get the details of an invitation
      operationId: cloudflare-organization-invites-api
      x-api-path-slug: organizationsorganization-identifierinvitesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organization Invites
  /organizations/:organization_identifier/members:
    get:
      summary: List all members of a organization
      description: List all members of a organization
      operationId: cloudflare-organization-members-api
      x-api-path-slug: organizationsorganization-identifiermembers-get
      responses:
        200:
          description: OK
      tags:
      - Organization Members
  /organizations/:organization_identifier/members/:identifier:
    delete:
      summary: Remove a member from an organization
      description: Remove a member from an organization
      operationId: cloudflare-organization-members-api
      x-api-path-slug: organizationsorganization-identifiermembersidentifier-delete
      responses:
        200:
          description: OK
      tags:
      - Organization Members
    get:
      summary: Get information about a specific member of an organization
      description: Get information about a specific member of an organization
      operationId: cloudflare-organization-members-api
      x-api-path-slug: organizationsorganization-identifiermembersidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organization Members
    patch:
      summary: Change the Roles of an Organization&#39;s Member
      description: Change the Roles of an Organization&#39;s Member
      operationId: cloudflare-organization-members-api
      x-api-path-slug: organizationsorganization-identifiermembersidentifier-patch
      parameters:
      - in: query
        name: roles
        description: Array of Roles associated with this Membertttttttttttttt[3536bcfad5faccb999b47003c79917fb]
      - in: header
        name: X-AUTH-EMAIL
        description: Email address associated with your account
      - in: header
        name: X-AUTH-KEY
        description: API key generated on the My Account page
      responses:
        200:
          description: OK
      tags:
      - Organization Members
  /organizations/:organization_identifier/roles:
    get:
      summary: Get all available roles for an organization
      description: Get all available roles for an organization
      operationId: cloudflare-organization-roles-api
      x-api-path-slug: organizationsorganization-identifierroles-get
      responses:
        200:
          description: OK
      tags:
      - Organization Roles
  /organizations/:organization_identifier/roles/:identifier:
    get:
      summary: Get information about a specific role for an organization
      description: Get information about a specific role for an organization
      operationId: cloudflare-organization-roles-api
      x-api-path-slug: organizationsorganization-identifierrolesidentifier-get
      responses:
        200:
          description: OK
      tags:
      - Organization Roles
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