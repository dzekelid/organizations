---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Get Organizations Name Oauth2 Accesstokens Access Token
  description: Gets details of a specific access token.
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
    put:
      summary: Put Organizations Name Developers Developer Name
      description: Update an existing developer profile with new values or additional
        attributes.
      operationId: putOrganizationsOrgNameDevelopersDeveloperName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-name-put
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: developer_name
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
    post:
      summary: Post Organizations Name Developers Developer Name
      description: Sets the status of a developer.
      operationId: postOrganizationsOrgNameDevelopersDeveloperName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-name-post
      parameters:
      - in: query
        name: action
        description: Set the status
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: developer_name
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
    delete:
      summary: Delete Organizations Name Developers Developer Name
      description: Deletes a developer from an Organization.
      operationId: deleteOrganizationsOrgNameDevelopersDeveloperName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-name-delete
      parameters:
      - in: path
        name: developer_name
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
  /organizations/{org_name}/developers/{developer_email}/apps:
    get:
      summary: Get Organizations Name Developers Developer Email Apps
      description: Provides an expanded view of a developer's collection of apps .
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailApps
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailapps-get
      parameters:
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: query
        name: expand
        description: Mention expand value as true
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - s
    post:
      summary: Post Organizations Name Developers Developer Email Apps
      description: Creates an app associated with a developer.
      operationId: postOrganizationsOrgNameDevelopersDeveloperEmailApps
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailapps-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - s
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name
      description: Gets a count of all API resources in the API products accessible
        by a developer app .
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-name-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: query
        name: entity
        description: Specify the entity as API resources
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: query
        description: Set query value to count
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
    put:
      summary: Put Organizations Name Developers Developer Email Apps App Name
      description: Updates the app to get a new set of consumer credentials.
      operationId: putOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-name-put
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
    post:
      summary: Post Organizations Name Developers Developer Email Apps App Name
      description: Revokes a Developer App, disabling access to all API Products .
      operationId: postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-name-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: path
        name: app_name
        description: Mention the app name
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
    delete:
      summary: Delete Organizations Name Developers Developer Email Apps App Name
      description: Delete a Developer's App.
      operationId: deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-name-delete
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key
      description: Returns details for a consumer key for a developer app .
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the Developer Email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
    post:
      summary: Post Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key
      description: Revokes a developer app key.
      operationId: postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: developer_email
        description: Mention the Developer Email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
    delete:
      summary: Delete Organizations Name Developers Developer Email Apps App Name
        Keys Consumer Key
      description: Deletes a consumer key that belongs to an app.
      operationId: deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-delete
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the Developer Email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/apiproducts/{apiproduct_name}:
    post:
      summary: Post Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key Apiproducts Apiproduct Name
      description: Revokes the association of an API Product with a Developer App's
        consumer key.
      operationId: postOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyApiproductsApiproductName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: path
        name: apiproduct_name
        description: Mention the API Product name
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the app name
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - API
      - Products
      - API
      - Productss
    delete:
      summary: Delete Organizations Name Developers Developer Email Apps App Name
        Keys Consumer Key Apiproducts Apiproduct Name
      description: Removes an API product from a developer app key profile, and thereby
        renders the developer app unable to access the URIs defined in the API product
        specified.
      operationId: deleteOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyApiproductsApiproductNam
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-delete
      parameters:
      - in: path
        name: apiproduct_name
        description: Mention the API Product name
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the app name
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - API
      - Products
      - API
      - Productss
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/oauth1accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Oauth1accesstokens
      description: Get count of OAuth 1.0 access tokens for a developer's app.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameOauth1accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth1accesstokens-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization Name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Oauth1accesstokens
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/oauth2accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Oauth2accesstokens
      description: Get count of    OAuth 2.0 access tokens for a developer's app.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameOauth2accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth2accesstokens-get
      parameters:
      - in: query
        name: appName
        description: Mention the app name
      - in: query
        name: developerEmail
        description: Mention the developer email
      - in: query
        name: organizationName
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Oauth2accesstokens
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth1accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key Oauth1accesstokens
      description: Get count of OAuth 1.0 access tokens for a developer's app key.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyOauth1accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth1accesstokens-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - Oauth1accesstokens
  /organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth2accesstokens:
    get:
      summary: Get Organizations Name Developers Developer Email Apps App Name Keys
        Consumer Key Oauth2accesstokens
      description: Get count of OAuth 2.0 access tokens for a developer's app key.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppsAppNameKeysConsumerKeyOauth2accesstokens
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth2accesstokens-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: developer_email
        description: Mention the developer name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Developers
      - Developer
      - Email
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
      - Oauth2accesstokens
  /organizations/{org_name}/oauth1/requesttokens/{request_token}:
    get:
      summary: Get Organizations Name Oauth1 Requesttokens Request Token
      description: Gets the Oauth 1.0 a request token for the speficied consumer key.
      operationId: getOrganizationsOrgNameOauth1RequesttokensRequestToken
      x-api-path-slug: organizationsorg-nameoauth1requesttokensrequest-token-get
      parameters:
      - in: query
        name: consumerKey
        description: Mention valid consumer key
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: request_token
        description: Mention the request token
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Requesttokens
      - Request
      - Token
    post:
      summary: Post Organizations Name Oauth1 Requesttokens Request Token
      description: Revokes an OAuth 1.0 a request token.
      operationId: postOrganizationsOrgNameOauth1RequesttokensRequestToken
      x-api-path-slug: organizationsorg-nameoauth1requesttokensrequest-token-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: request_token
        description: Mention the request token
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Requesttokens
      - Request
      - Token
    delete:
      summary: Delete Organizations Name Oauth1 Requesttokens Request Token
      description: Deletes the request token specified.
      operationId: deleteOrganizationsOrgNameOauth1RequesttokensRequestToken
      x-api-path-slug: organizationsorg-nameoauth1requesttokensrequest-token-delete
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: request_token
        description: Mention the request token
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Requesttokens
      - Request
      - Token
  /organizations/{org_name}/oauth1/requesttokens:
    get:
      summary: Get Organizations Name Oauth1 Requesttokens
      description: Returns list of all OAuth 1.0a request.
      operationId: getOrganizationsOrgNameOauth1Requesttokens
      x-api-path-slug: organizationsorg-nameoauth1requesttokens-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Requesttokens
  /organizations/{org_name}/oauth1/verifiers/{verifier_code}:
    get:
      summary: Get Organizations Name Oauth1 Verifiers Verifier Code
      description: Gets the detail of given verifier code.
      operationId: getOrganizationsOrgNameOauth1VerifiersVerifierCode
      x-api-path-slug: organizationsorg-nameoauth1verifiersverifier-code-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: verifier_code
        description: Mention the verifier code
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Verifiers
      - Verifier
      - Code
    delete:
      summary: Delete Organizations Name Oauth1 Verifiers Verifier Code
      description: Deletes the specified verifier code, which is the verifier code
        given by the provider.
      operationId: deleteOrganizationsOrgNameOauth1VerifiersVerifierCode
      x-api-path-slug: organizationsorg-nameoauth1verifiersverifier-code-delete
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: verifier_code
        description: Mention the verifier code
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Verifiers
      - Verifier
      - Code
  /organizations/{org_name}/oauth1/verifiers:
    get:
      summary: Get Organizations Name Oauth1 Verifiers
      description: Gets a list of all verifiers and details for each verifier in an
        Organization.
      operationId: getOrganizationsOrgNameOauth1Verifiers
      x-api-path-slug: organizationsorg-nameoauth1verifiers-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Verifiers
  /organizations/{org_name}/oauth1/accesstokens/{access_token}:
    get:
      summary: Get Organizations Name Oauth1 Accesstokens Access Token
      description: Fetches the details of given access token.
      operationId: getOrganizationsOrgNameOauth1AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth1accesstokensaccess-token-get
      parameters:
      - in: path
        name: access_token
        description: Mention the access token
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Accesstokens
      - Access
      - Token
    post:
      summary: Post Organizations Name Oauth1 Accesstokens Access Token
      description: Revokes the specified access token.
      operationId: postOrganizationsOrgNameOauth1AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth1accesstokensaccess-token-post
      parameters:
      - in: path
        name: access_token
        description: Mention the access token
      - in: query
        name: action
        description: Mention action as revoke
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Accesstokens
      - Access
      - Token
    delete:
      summary: Delete Organizations Name Oauth1 Accesstokens Access Token
      description: Deletes the specified access token.
      operationId: deleteOrganizationsOrgNameOauth1AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth1accesstokensaccess-token-delete
      parameters:
      - in: path
        name: access_token
        description: Mention the access token
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Accesstokens
      - Access
      - Token
  /organizations/{org_name}/oauth1/accesstokens:
    get:
      summary: Get Organizations Name Oauth1 Accesstokens
      description: Returns a count of all 1.0a access tokens in an orgnization .
      operationId: getOrganizationsOrgNameOauth1Accesstokens
      x-api-path-slug: organizationsorg-nameoauth1accesstokens-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth1
      - Accesstokens
  /organizations/{org_name}/oauth2/authorizationcodes/{authorization_code}:
    get:
      summary: Get Organizations Name Oauth2 Authorizationcodes Authorization Code
      description: Get a specific Authorization Code.
      operationId: getOrganizationsOrgNameOauth2AuthorizationcodesAuthorizationCode
      x-api-path-slug: organizationsorg-nameoauth2authorizationcodesauthorization-code-get
      parameters:
      - in: path
        name: authorization_code
        description: Mention the auth code
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth2
      - Authorizationcodes
      - Authorization
      - Code
    delete:
      summary: Delete Organizations Name Oauth2 Authorizationcodes Authorization Code
      description: Deletes the given authorization Code.
      operationId: deleteOrganizationsOrgNameOauth2AuthorizationcodesAuthorizationCode
      x-api-path-slug: organizationsorg-nameoauth2authorizationcodesauthorization-code-delete
      parameters:
      - in: path
        name: authorization_code
        description: Mention the auth code
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth2
      - Authorizationcodes
      - Authorization
      - Code
  /organizations/{org_name}/oauth2/authorizationcodes:
    get:
      summary: Get Organizations Name Oauth2 Authorizationcodes
      description: Lists all authorization codes in an organization.
      operationId: getOrganizationsOrgNameOauth2Authorizationcodes
      x-api-path-slug: organizationsorg-nameoauth2authorizationcodes-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth2
      - Authorizationcodes
  /organizations/{org_name}/oauth2/accesstokens/{access_token}:
    get:
      summary: Get Organizations Name Oauth2 Accesstokens Access Token
      description: Gets details of a specific access token.
      operationId: getOrganizationsOrgNameOauth2AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth2accesstokensaccess-token-get
      parameters:
      - in: path
        name: access_token
        description: Mention the Access Token
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Oauth2
      - Accesstokens
      - Access
      - Token
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