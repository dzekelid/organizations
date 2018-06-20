---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Get Organizations Name Developers Developer Name
  description: Get a count of apps by developer email address.
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations:
    get:
      summary: Get Organizations
      description: Lists all the organizations.
      operationId: getOrganizations
      x-api-path-slug: organizations-get
      responses:
        200:
          description: OK
      tags:
      - Organizations
    post:
      summary: Post Organizations
      description: Creates an organization.
      operationId: postOrganizations
      x-api-path-slug: organizations-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/{org_name}:
    get:
      summary: Get Organizations Name
      description: Gets a specific organization.
      operationId: getOrganizationsOrgName
      x-api-path-slug: organizationsorg-name-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
    put:
      summary: Put Organizations Name
      description: Updates the description of a specific organization.
      operationId: putOrganizationsOrgName
      x-api-path-slug: organizationsorg-name-put
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
    delete:
      summary: Delete Organizations Name
      description: Deletes a specific organization.
      operationId: deleteOrganizationsOrgName
      x-api-path-slug: organizationsorg-name-delete
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/{org_name}/deployments:
    get:
      summary: Get Organizations Name Deployments
      description: Gets all deployments of an organization.
      operationId: getOrganizationsOrgNameDeployments
      x-api-path-slug: organizationsorg-namedeployments-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Deployments
  /organizations/{org_name}/pods:
    get:
      summary: Get Organizations Name Pods
      description: Gets all the pods associated with an organization.
      operationId: getOrganizationsOrgNamePods
      x-api-path-slug: organizationsorg-namepods-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Pods
    post:
      summary: Post Organizations Name Pods
      description: Disassociates a pod from an organization.
      operationId: postOrganizationsOrgNamePods
      x-api-path-slug: organizationsorg-namepods-post
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Pods
  /organizations/{org_name}/environments:
    get:
      summary: Get Organizations Name Environments
      description: Lists all the environments in an organization.
      operationId: getOrganizationsOrgNameEnvironments
      x-api-path-slug: organizationsorg-nameenvironments-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
    post:
      summary: Post Organizations Name Environments
      description: Creates an environment.
      operationId: postOrganizationsOrgNameEnvironments
      x-api-path-slug: organizationsorg-nameenvironments-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
  /organizations/{org_name}/environments/{env_name}:
    get:
      summary: Get Organizations Name Environments Env Name
      description: Gets details for an environment.
      operationId: getOrganizationsOrgNameEnvironmentsEnvName
      x-api-path-slug: organizationsorg-nameenvironmentsenv-name-get
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
    post:
      summary: Post Organizations Name Environments Env Name
      description: Updates an environment.
      operationId: postOrganizationsOrgNameEnvironmentsEnvName
      x-api-path-slug: organizationsorg-nameenvironmentsenv-name-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
    delete:
      summary: Delete Organizations Name Environments Env Name
      description: Deletes a specific environment in an organization.
      operationId: deleteOrganizationsOrgNameEnvironmentsEnvName
      x-api-path-slug: organizationsorg-nameenvironmentsenv-name-delete
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
  /organizations/{org_name}/environments/{env_name}/deployments:
    get:
      summary: Get Organizations Name Environments Env Name Deployments
      description: Gets the deployments for an environment in an organization.
      operationId: getOrganizationsOrgNameEnvironmentsEnvNameDeployments
      x-api-path-slug: organizationsorg-nameenvironmentsenv-namedeployments-get
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Deployments
  /organizations/{org_name}/environments/{env_name}/apis/{api_name}/deployments:
    get:
      summary: Get Organizations Name Environments Env Name API Name Deployments
      description: Gets the deployments for an API Proxy in the given environment
        in an organization.
      operationId: getOrganizationsOrgNameEnvironmentsEnvNameApisApiNameDeployments
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameapisapi-namedeployments-get
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Envs
      - APIs
      - Deployments
  /organizations/{org_name}/environments/{env_name}/apis/{api_name}/revisions/{revision_number}/deployments:
    get:
      summary: Get Organizations Name Environments Env Name API Name Revisions Revision
        Number Deployments
      description: "Gets the deployments for an API Proxy\xE2\x80\x99s revision for
        an environment in an organization."
      operationId: getOrganizationsOrgNameEnvironmentsEnvNameApisApiNameRevisionsRevisionNumberDeployments
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameapisapi-namerevisionsrevision-numberdeployments-get
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: revision_number
        description: Mention the revision
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Envs
      - APIs
      - Revisions
      - Revision
      - Number
      - Deployments
  /organizations/{org_name}/environments/{env_name}/servers:
    get:
      summary: Get Organizations Name Environments Env Name Servers
      description: Gets the servers that are bound to an environment.
      operationId: getOrganizationsOrgNameEnvironmentsEnvNameServers
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameservers-get
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Servers
    post:
      summary: Post Organizations Name Environments Env Name Servers
      description: Add servers into the environment.
      operationId: postOrganizationsOrgNameEnvironmentsEnvNameServers
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameservers-post
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Servers
    delete:
      summary: Delete Organizations Name Environments Env Name Servers
      description: Deletes servers from the environment.
      operationId: deleteOrganizationsOrgNameEnvironmentsEnvNameServers
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameservers-delete
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Servers
  /organizations/{org_name}/environments/{env_name}/virtualhosts:
    get:
      summary: Get Organizations Name Environments Env Name Virtualhosts
      description: Lists all virtual hosts in an environment.
      operationId: getOrganizationsOrgNameEnvironmentsEnvNameVirtualhosts
      x-api-path-slug: organizationsorg-nameenvironmentsenv-namevirtualhosts-get
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Virtualhosts
    post:
      summary: Post Organizations Name Environments Env Name Virtualhosts
      description: Creates a virtual host.
      operationId: postOrganizationsOrgNameEnvironmentsEnvNameVirtualhosts
      x-api-path-slug: organizationsorg-nameenvironmentsenv-namevirtualhosts-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Virtualhosts
  /organizations/{org_name}/environments/{env_name}/virtualhosts/{virtualhost_name}:
    get:
      summary: Get Organizations Name Environments Env Name Virtualhosts Virtualhost
        Name
      description: Gets details for a named virtual host .
      operationId: getOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName
      x-api-path-slug: organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-get
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: virtualhost_name
        description: Mention the virtual host name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Virtualhosts
      - Virtualhost
    post:
      summary: Post Organizations Name Environments Env Name Virtualhosts Virtualhost
        Name
      description: Updates a specific virtual host in an environment.
      operationId: postOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName
      x-api-path-slug: organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: virtualhost_name
        description: Mention the virtual host name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Virtualhosts
      - Virtualhost
    delete:
      summary: Delete Organizations Name Environments Env Name Virtualhosts Virtualhost
        Name
      description: Deletes a specific virtual host in an environment.
      operationId: deleteOrganizationsOrgNameEnvironmentsEnvNameVirtualhostsVirtualhostName
      x-api-path-slug: organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-delete
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: virtualhost_name
        description: Mention the virtual host name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Virtualhosts
      - Virtualhost
  /organizations/{org_name}/apis/{api_name}/revisions/{revision_number}/deployments:
    post:
      summary: Post Organizations Name API Name Revisions Revision Number Deployments
      description: Undeploys an API proxy revision from an environment.
      operationId: postOrganizationsOrgNameApisApiNameRevisionsRevisionNumberDeployments
      x-api-path-slug: organizationsorg-nameapisapi-namerevisionsrevision-numberdeployments-post
      parameters:
      - in: query
        name: action
        description: Specify the action
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: env
        description: Specify environment name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: revision_number
        description: Mention the API Proxy revision number
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
      - Revisions
      - Revision
      - Number
      - Deployments
  /organizations/{org_name}/apis:
    get:
      summary: Get Organizations Name APIs
      description: Gets all APIs in an organization.
      operationId: getOrganizationsOrgNameApis
      x-api-path-slug: organizationsorg-nameapis-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - APIs
    post:
      summary: Post Organizations Name APIs
      description: Uploads a ZIP-formatted API proxy configuration bundle from a local
        machine to an organization on the API Platform.
      operationId: postOrganizationsOrgNameApis
      x-api-path-slug: organizationsorg-nameapis-post
      parameters:
      - in: query
        name: action
        description: Specify the action
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: name
        description: Specify API Proxy name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - APIs
  /organizations/{org_name}/apis/{api_name}:
    get:
      summary: Get Organizations Name API Name
      description: Gets an API proxy by name, providing a list of existing revisions
        of the API proxy configuration.
      operationId: getOrganizationsOrgNameApisApiName
      x-api-path-slug: organizationsorg-nameapisapi-name-get
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
    delete:
      summary: Delete Organizations Name API Name
      description: Deletes an API and all associated endpoints, policies, resources,
        and revisions.
      operationId: deleteOrganizationsOrgNameApisApiName
      x-api-path-slug: organizationsorg-nameapisapi-name-delete
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
  /organizations/{org_name}/apis/{api_name}/revisions/revision_number:
    put:
      summary: Put Organizations Name API Name Revisions Revision Number
      description: Use the POST method to update a specific API proxy in an organization.
      operationId: putOrganizationsOrgNameApisApiNameRevisionsRevisionNumber
      x-api-path-slug: organizationsorg-nameapisapi-namerevisionsrevision-number-put
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: revision_number
        description: Mention the revision number
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
      - Revisions
      - Revision
      - Number
  /organizations/{org_name}/apis/{api_name}/revisions/{revision_number}:
    get:
      summary: Get Organizations Name API Name Revisions Revision Number
      description: Exports an API from Apigee to the local machine a ZIP bundle of
        config and code files..
      operationId: getOrganizationsOrgNameApisApiNameRevisionsRevisionNumber
      x-api-path-slug: organizationsorg-nameapisapi-namerevisionsrevision-number-get
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: query
        name: format
        description: RESTful management API to create, configure, and manage API proxies
          and API products, create and manage apps and app developers, and more
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: revision_number
        description: Mention the API Proxy revision
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
      - Revisions
      - Revision
      - Number
    delete:
      summary: Delete Organizations Name API Name Revisions Revision Number
      description: Deletes a specific revision of an API.
      operationId: deleteOrganizationsOrgNameApisApiNameRevisionsRevisionNumber
      x-api-path-slug: organizationsorg-nameapisapi-namerevisionsrevision-number-delete
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: revision_number
        description: Mention the API Proxy revision
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
      - Revisions
      - Revision
      - Number
  /organizations/{org_name}/apis/{api_name}/deployments:
    get:
      summary: Get Organizations Name API Name Deployments
      description: Returns detail on deployments of the API specified.
      operationId: getOrganizationsOrgNameApisApiNameDeployments
      x-api-path-slug: organizationsorg-nameapisapi-namedeployments-get
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
      - Deployments
  /organizations/{org_name}/apis/{api_name}/revisions/{revision_name}/deployments:
    get:
      summary: Get Organizations Name API Name Revisions Revision Name Deployments
      description: Get deployments for a revision of an API proxy.
      operationId: getOrganizationsOrgNameApisApiNameRevisionsRevisionNameDeployments
      x-api-path-slug: organizationsorg-nameapisapi-namerevisionsrevision-namedeployments-get
      parameters:
      - in: path
        name: api_name
        description: Mention the API Proxy name
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: revision_number
        description: Mention the API Proxy revision
      responses:
        200:
          description: OK
      tags:
      - Organizationss
      - APIs
      - Revisions
      - Revision
      - Deployments
  /organizations/{org_name}/apiproducts:
    get:
      summary: Get Organizations Name Apiproducts
      description: Lists all API products by name for an organization.
      operationId: getOrganizationsOrgNameApiproducts
      x-api-path-slug: organizationsorg-nameapiproducts-get
      parameters:
      - in: path
        name: org_name
        description: Mention the Organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - API
      - Products
    post:
      summary: Post Organizations Name Apiproducts
      description: 'Create an API product: a list of API resources combined with Quota
        settings that you can use to deliver customized API bundles to your developers.'
      operationId: postOrganizationsOrgNameApiproducts
      x-api-path-slug: organizationsorg-nameapiproducts-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: org_name
        description: Mention the Organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - API
      - Products
  /organizations/{org_name}/apiproducts/{apiproduct_name}:
    get:
      summary: Get Organizations Name Apiproducts Apiproduct Name
      description: Gets the list of keys/apps/developers for an API product of an
        organization.
      operationId: getOrganizationsOrgNameApiproductsApiproductName
      x-api-path-slug: organizationsorg-nameapiproductsapiproduct-name-get
      parameters:
      - in: path
        name: apiproduct_name
        description: Mention the API Product name
      - in: query
        name: entity
        description: Specify the entity
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: query
        description: Query type count
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - API
      - Products
      - API
      - Productss
    put:
      summary: Put Organizations Name Apiproducts Apiproduct Name
      description: This method updates an existing API product.
      operationId: putOrganizationsOrgNameApiproductsApiproductName
      x-api-path-slug: organizationsorg-nameapiproductsapiproduct-name-put
      parameters:
      - in: path
        name: apiproduct_name
        description: Mention the API Product name
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - API
      - Products
      - API
      - Productss
    delete:
      summary: Delete Organizations Name Apiproducts Apiproduct Name
      description: Deletes an API product.
      operationId: deleteOrganizationsOrgNameApiproductsApiproductName
      x-api-path-slug: organizationsorg-nameapiproductsapiproduct-name-delete
      parameters:
      - in: path
        name: apiproduct_name
        description: Mention the API Product name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - API
      - Products
      - API
      - Productss
  /organizations/{org_name}/developers:
    get:
      summary: Get Organizations Name Developers
      description: Gets the developer profile by registered date.
      operationId: getOrganizationsOrgNameDevelopers
      x-api-path-slug: organizationsorg-namedevelopers-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: registeredat
        description: Mention the registered date
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
    post:
      summary: Post Organizations Name Developers
      description: Create a developer in an organization .
      operationId: postOrganizationsOrgNameDevelopers
      x-api-path-slug: organizationsorg-namedevelopers-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
  /organizations/{org_name}/developers/{developer_name}:
    get:
      summary: Get Organizations Name Developers Developer Name
      description: Get a count of apps by developer email address.
      operationId: getOrganizationsOrgNameDevelopersDeveloperName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-name-get
      parameters:
      - in: path
        name: developer_name
        description: Mention the developer email
      - in: query
        name: entity
        description: Specify the entity
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: query
        description: Query type count
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
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