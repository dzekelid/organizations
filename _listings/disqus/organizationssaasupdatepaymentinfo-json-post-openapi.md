---
swagger: "2.0"
x-collection-name: Disqus
x-complete: 0
info:
  title: Disqus Organizations Saas UpdatePaymentInfo
  description: Organizations Saas UpdatePaymentInfo
  termsOfService: https://docs.disqus.com/kb/terms-and-policies/
  version: 1.0.0
host: disqus.com
basePath: api/3.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/listAdmins.json:
    get:
      summary: Organizations ListAdmins
      description: Organizations ListAdmins
      operationId: organizations-listadmins
      x-api-path-slug: organizationslistadmins-json-get
      parameters:
      - in: query
        name: organization
        description: Looks up an organization by ID You must be an admin on the selected
          organization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Organizations
  /organizations/removeAdmin.json:
    post:
      summary: Organizations RemoveAdmin
      description: Organizations RemoveAdmin
      operationId: organizations-removeadmin
      x-api-path-slug: organizationsremoveadmin-json-post
      parameters:
      - in: query
        name: organization
        description: Looks up an organization by ID You must be an admin on the selected
          organization
        type: string
      - in: query
        name: user
        description: Looks up a user by ID You may look up a user by username using
          the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Organizations
  /organizations/setRole.json:
    post:
      summary: Organizations SetRole
      description: Organizations SetRole
      operationId: organizations-setrole
      x-api-path-slug: organizationssetrole-json-post
      parameters:
      - in: query
        name: isAdmin
        description: Defaults to null
        type: string
      - in: query
        name: isModerator
        description: Defaults to null
        type: string
      - in: query
        name: organization
        description: Looks up an organization by ID You must be an admin on the selected
          organization
        type: string
      - in: query
        name: user
        description: Looks up a user by ID You may look up a user by username using
          the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Organizations
  /organizations/saas/currentPlan.json:
    get:
      summary: Organizations Saas CurrentPlan
      description: Organizations Saas CurrentPlan
      operationId: organizations-saas-currentplan
      x-api-path-slug: organizationssaascurrentplan-json-get
      parameters:
      - in: query
        name: organization
        description: Looks up an organization by ID You must be an admin on the selected
          organization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Organizations
  /organizations/saas/removePaymentInfo.json:
    post:
      summary: Organizations Saas RemovePaymentInfo
      description: Organizations Saas RemovePaymentInfo
      operationId: organizations-saas-removepaymentinfo
      x-api-path-slug: organizationssaasremovepaymentinfo-json-post
      parameters:
      - in: query
        name: organization
        description: Looks up an organization by ID You must be an admin on the selected
          organization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Organizations
  /organizations/saas/subscribe.json:
    post:
      summary: Organizations Saas Subscribe
      description: Organizations Saas Subscribe
      operationId: organizations-saas-subscribe
      x-api-path-slug: organizationssaassubscribe-json-post
      parameters:
      - in: query
        name: organization
        description: Looks up an organization by ID You must be an admin on the selected
          organization
        type: string
      - in: query
        name: plan
        description: Looks up a PricingOption by name
        type: string
      - in: query
        name: user
        description: Defaults to null                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Organizations
  /organizations/saas/unsubscribe.json:
    post:
      summary: Organizations Saas Unsubscribe
      description: Organizations Saas Unsubscribe
      operationId: organizations-saas-unsubscribe
      x-api-path-slug: organizationssaasunsubscribe-json-post
      parameters:
      - in: query
        name: immediately
        description: Defaults to false
        type: string
      - in: query
        name: organization
        description: Looks up an organization by ID You must be an admin on the selected
          organization
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Organizations
  /organizations/saas/updatePaymentInfo.json:
    post:
      summary: Organizations Saas UpdatePaymentInfo
      description: Organizations Saas UpdatePaymentInfo
      operationId: organizations-saas-updatepaymentinfo
      x-api-path-slug: organizationssaasupdatepaymentinfo-json-post
      parameters:
      - in: query
        name: organization
        description: Looks up an organization by ID You must be an admin on the selected
          organization
        type: string
      - in: query
        name: token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Organizations
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