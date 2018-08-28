---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Delete Organizations Org
  description: Delete a organization given its identifier
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/:
    get:
      summary: Get Organizations
      description: List or search all organizations
      operationId: getOrganizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: badge
      - in: query
        name: datasets
      - in: query
        name: facets
        description: Selected facets to fetch
      - in: query
        name: followers
      - in: query
        name: page
        description: The page to display
      - in: query
        name: page_size
        description: The page size
      - in: query
        name: permitted_reuses
      - in: query
        name: q
        description: The search query
      - in: query
        name: reuses
      - in: query
        name: sort
        description: The field (and direction) on which sorting apply
      responses:
        200:
          description: OK
      tags:
      - Organizations
    post:
      summary: Add Organizations
      description: Create a new organization
      operationId: postOrganizations
      x-api-path-slug: organizations-post
      parameters:
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/badges/:
    get:
      summary: Get Organizations Badges
      description: List all available organization badges and their labels
      operationId: getOrganizationsBadges
      x-api-path-slug: organizationsbadges-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Badges
  /organizations/suggest/:
    get:
      summary: Get Organizations Suggest
      description: Suggest organizations
      operationId: getOrganizationsSuggest
      x-api-path-slug: organizationssuggest-get
      parameters:
      - in: query
        name: q
        description: The string to autocomplete/suggest
      - in: query
        name: size
        description: The amount of suggestion to fetch
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Suggest
  /organizations/{id}/followers/:
    delete:
      summary: Delete Organizations  Followers
      description: Unfollow an object given its ID
      operationId: deleteOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
    get:
      summary: Get Organizations  Followers
      description: List all followers for a given object
      operationId: getOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-get
      parameters:
      - in: path
        name: id
      - in: query
        name: page
        description: The page to fetch
      - in: query
        name: page_size
        description: The page size to fetch
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
    post:
      summary: Add Organizations  Followers
      description: Follow an object given its ID
      operationId: postOrganizationsFollowers
      x-api-path-slug: organizationsidfollowers-post
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - ""
      - Followers
  /organizations/{org}/:
    delete:
      summary: Delete Organizations Org
      description: Delete a organization given its identifier
      operationId: deleteOrganizationsOrg
      x-api-path-slug: organizationsorg-delete
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
    get:
      summary: Get Organizations Org
      description: Get a organization given its identifier
      operationId: getOrganizationsOrg
      x-api-path-slug: organizationsorg-get
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
    put:
      summary: Put Organizations Org
      description: Update a organization given its identifier
      operationId: putOrganizationsOrg
      x-api-path-slug: organizationsorg-put
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
  /organizations/{org}/badges/:
    post:
      summary: Add Organizations Org Badges
      description: Create a new badge for a given organization
      operationId: postOrganizationsOrgBadges
      x-api-path-slug: organizationsorgbadges-post
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Badges
  /organizations/{org}/badges/{badge_kind}/:
    delete:
      summary: Delete Organizations Org Badges Badge Kind
      description: Delete a badge for a given organization
      operationId: deleteOrganizationsOrgBadgesBadgeKind
      x-api-path-slug: organizationsorgbadgesbadge-kind-delete
      parameters:
      - in: path
        name: badge_kind
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Badges
      - Badge
      - Kind
  /organizations/{org}/datasets/:
    get:
      summary: Get Organizations Org Datasets
      description: List organization datasets (including private ones when member)
      operationId: getOrganizationsOrgDatasets
      x-api-path-slug: organizationsorgdatasets-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Datasets
  /organizations/{org}/discussions/:
    get:
      summary: Get Organizations Org Discussions
      description: List organization discussions
      operationId: getOrganizationsOrgDiscussions
      x-api-path-slug: organizationsorgdiscussions-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Discussions
  /organizations/{org}/issues/:
    get:
      summary: Get Organizations Org Issues
      description: List organization issues
      operationId: getOrganizationsOrgIssues
      x-api-path-slug: organizationsorgissues-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Issues
  /organizations/{org}/logo:
    post:
      summary: Add Organizations Org Logo
      description: Upload a new logo
      operationId: postOrganizationsOrgLogo
      x-api-path-slug: organizationsorglogo-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Logo
    put:
      summary: Put Organizations Org Logo
      description: Set the logo BBox
      operationId: putOrganizationsOrgLogo
      x-api-path-slug: organizationsorglogo-put
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Logo
  /organizations/{org}/member/{user}:
    delete:
      summary: Delete Organizations Org Member User
      description: Delete member from an organization
      operationId: deleteOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-delete
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
    post:
      summary: Add Organizations Org Member User
      description: Add a member into a given organization
      operationId: postOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-post
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
    put:
      summary: Put Organizations Org Member User
      description: Update member status into a given organization
      operationId: putOrganizationsOrgMemberUser
      x-api-path-slug: organizationsorgmemberuser-put
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Member
      - User
  /organizations/{org}/membership/:
    get:
      summary: Get Organizations Org Membership
      description: List membership requests for a given organization
      operationId: getOrganizationsOrgMembership
      x-api-path-slug: organizationsorgmembership-get
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      - in: query
        name: status
        description: If provided, only return requests ith a given status
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
    post:
      summary: Add Organizations Org Membership
      description: Apply for membership to a given organization
      operationId: postOrganizationsOrgMembership
      x-api-path-slug: organizationsorgmembership-post
      parameters:
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
  /organizations/{org}/membership/{id}/accept/:
    post:
      summary: Add Organizations Org Membership  Accept
      description: Accept user membership to a given organization
      operationId: postOrganizationsOrgMembershipAccept
      x-api-path-slug: organizationsorgmembershipidaccept-post
      parameters:
      - in: path
        name: id
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
      - ""
      - Accept
  /organizations/{org}/membership/{id}/refuse/:
    post:
      summary: Add Organizations Org Membership  Refuse
      description: Refuse user membership to a given organization
      operationId: postOrganizationsOrgMembershipRefuse
      x-api-path-slug: organizationsorgmembershipidrefuse-post
      parameters:
      - in: body
        name: comment
        description: The refusal reason
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: org
        description: The organization ID or slug
      - in: body
        name: payload
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Membership
      - ""
      - Refuse
  /organizations/{org}/reuses/:
    get:
      summary: Get Organizations Org Reuses
      description: List organization reuses (including private ones when member)
      operationId: getOrganizationsOrgReuses
      x-api-path-slug: organizationsorgreuses-get
      parameters:
      - in: path
        name: org
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Reuses
  /me/org_community_resources/:
    get:
      summary: Get Me Org Community Resources
      description: List all community resources related to me and my organizations
      operationId: getMeOrgCommunityResources
      x-api-path-slug: meorg-community-resources-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Community
      - Resources
  /me/org_datasets/:
    get:
      summary: Get Me Org Datasets
      description: List all datasets related to me and my organizations
      operationId: getMeOrgDatasets
      x-api-path-slug: meorg-datasets-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Datasets
  /me/org_discussions/:
    get:
      summary: Get Me Org Discussions
      description: List all discussions related to my organizations
      operationId: getMeOrgDiscussions
      x-api-path-slug: meorg-discussions-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Discussions
  /me/org_issues/:
    get:
      summary: Get Me Org Issues
      description: List all issues related to my organizations
      operationId: getMeOrgIssues
      x-api-path-slug: meorg-issues-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Issues
  /me/org_reuses/:
    get:
      summary: Get Me Org Reuses
      description: List all reuses related to me and my organizations
      operationId: getMeOrgReuses
      x-api-path-slug: meorg-reuses-get
      parameters:
      - in: query
        name: q
        description: The string to filter items
      responses:
        200:
          description: OK
      tags:
      - Me
      - Org
      - Reuses
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