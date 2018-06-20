---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 1
info:
  title: Apigee Edge
  description: restful-management-api-to-create-configure-and-manage-api-proxies-and-api-products-create-and-manage-apps-and-app-developers-and-more-
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
    post:
      summary: Post Organizations Name Oauth2 Accesstokens Access Token
      description: Revokes a specific access token.
      operationId: postOrganizationsOrgNameOauth2AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth2accesstokensaccess-token-post
      parameters:
      - in: path
        name: access_token
        description: Mention the Access Token
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
      - Oauth2
      - Accesstokens
      - Access
      - Token
    delete:
      summary: Delete Organizations Name Oauth2 Accesstokens Access Token
      description: Deletes a specific access token.
      operationId: deleteOrganizationsOrgNameOauth2AccesstokensAccessToken
      x-api-path-slug: organizationsorg-nameoauth2accesstokensaccess-token-delete
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
  /organizations/{org_name}/oauth2/accesstokens:
    get:
      summary: Get Organizations Name Oauth2 Accesstokens
      description: Get count of OAuth 2.0 access tokens under an organization .
      operationId: getOrganizationsOrgNameOauth2Accesstokens
      x-api-path-slug: organizationsorg-nameoauth2accesstokens-get
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
      - Accesstokens
  /organizations/{org_name}/keyvaluemaps:
    get:
      summary: Get Organizations Name Keyvaluemaps
      description: Returns an expanded view of all Maps scoped by organization, environment
        or API.
      operationId: getOrganizationsOrgNameKeyvaluemaps
      x-api-path-slug: organizationsorg-namekeyvaluemaps-get
      parameters:
      - in: query
        name: expand
        description: Set expand value to true
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
    post:
      summary: Post Organizations Name Keyvaluemaps
      description: Creates a KeyValueMap.
      operationId: postOrganizationsOrgNameKeyvaluemaps
      x-api-path-slug: organizationsorg-namekeyvaluemaps-post
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
      - Keyvaluemaps
  /organizations/{org_name}/keyvaluemaps/{map_name}/entries/{entry_name}:
    get:
      summary: Get Organizations Name Keyvaluemaps Map Name Entries Entry Name
      description: Gets a specific entry details.
      operationId: getOrganizationsOrgNameKeyvaluemapsMapNameEntriesEntryName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-nameentriesentry-name-get
      parameters:
      - in: path
        name: entry_name
        description: Mention the entry name
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
      - Entries
      - Entry
    delete:
      summary: Delete Organizations Name Keyvaluemaps Map Name Entries Entry Name
      description: Deletes a single entry by name.
      operationId: deleteOrganizationsOrgNameKeyvaluemapsMapNameEntriesEntryName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-nameentriesentry-name-delete
      parameters:
      - in: path
        name: entry_name
        description: Mention the entry name
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
      - Entries
      - Entry
  /organizations/{org_name}/keyvaluemaps/{map_name}:
    get:
      summary: Get Organizations Name Keyvaluemaps Map Name
      description: Gets a KeyValueMap by name, along with associated entries.
      operationId: getOrganizationsOrgNameKeyvaluemapsMapName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-name-get
      parameters:
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
    put:
      summary: Put Organizations Name Keyvaluemaps Map Name
      description: Updates an existing KeyValueMap.
      operationId: putOrganizationsOrgNameKeyvaluemapsMapName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-name-put
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
    delete:
      summary: Delete Organizations Name Keyvaluemaps Map Name
      description: Deletes a KeyValueMap and all associated entries.
      operationId: deleteOrganizationsOrgNameKeyvaluemapsMapName
      x-api-path-slug: organizationsorg-namekeyvaluemapsmap-name-delete
      parameters:
      - in: path
        name: map_name
        description: Mention the map name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Keyvaluemaps
      - Map
  /organizations/{org_name}/companies:
    get:
      summary: Get Organizations Name Companies
      description: Returns an expanded list of companies, displaying a full profile
        for each company in the organization.
      operationId: getOrganizationsOrgNameCompanies
      x-api-path-slug: organizationsorg-namecompanies-get
      parameters:
      - in: query
        name: expand
        description: Specify the Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
    post:
      summary: Post Organizations Name Companies
      description: Creates a company in an organization.
      operationId: postOrganizationsOrgNameCompanies
      x-api-path-slug: organizationsorg-namecompanies-post
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
      - Companies
  /organizations/{org_name}/companies/{company_name}:
    get:
      summary: Get Organizations Name Companies Company Name
      description: Gets details for a Company.
      operationId: getOrganizationsOrgNameCompaniesCompanyName
      x-api-path-slug: organizationsorg-namecompaniescompany-name-get
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
    put:
      summary: Put Organizations Name Companies Company Name
      description: Updates an existing Company.
      operationId: putOrganizationsOrgNameCompaniesCompanyName
      x-api-path-slug: organizationsorg-namecompaniescompany-name-put
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
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
      - Companies
      - Companies
    delete:
      summary: Delete Organizations Name Companies Company Name
      description: Deletes an existing Company.
      operationId: deleteOrganizationsOrgNameCompaniesCompanyName
      x-api-path-slug: organizationsorg-namecompaniescompany-name-delete
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
  /organizations/{org_name}/companies/{company_name}/developers:
    get:
      summary: Get Organizations Name Companies Company Name Developers
      description: Lists all developers associated with a company.
      operationId: getOrganizationsOrgNameCompaniesCompanyNameDevelopers
      x-api-path-slug: organizationsorg-namecompaniescompany-namedevelopers-get
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Developers
    post:
      summary: Post Organizations Name Companies Company Name Developers
      description: Adds a developer to a company.
      operationId: postOrganizationsOrgNameCompaniesCompanyNameDevelopers
      x-api-path-slug: organizationsorg-namecompaniescompany-namedevelopers-post
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
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
      - Companies
      - Companies
      - Developers
  /organizations/{org_name}/companies/{company_name}/developers/{developer_email}:
    delete:
      summary: Delete Organizations Name Companies Company Name Developers Developer
        Email
      description: Removes the association of a Developer with a Company.
      operationId: deleteOrganizationsOrgNameCompaniesCompanyNameDevelopersDeveloperEmail
      x-api-path-slug: organizationsorg-namecompaniescompany-namedevelopersdeveloper-email-delete
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
      - in: query
        name: Developer_email
        description: Mention the developer email
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Developers
      - Developer
      - Email
  /organizations/{org_name}/companies/{company_name}/apps:
    get:
      summary: Get Organizations Name Companies Company Name Apps
      description: Gets an expanded list company apps .
      operationId: getOrganizationsOrgNameCompaniesCompanyNameApps
      x-api-path-slug: organizationsorg-namecompaniescompany-nameapps-get
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
      - in: query
        name: expand
        description: Specify expand value as true
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - s
    post:
      summary: Post Organizations Name Companies Company Name Apps
      description: Creates an app for a company.
      operationId: postOrganizationsOrgNameCompaniesCompanyNameApps
      x-api-path-slug: organizationsorg-namecompaniescompany-nameapps-post
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
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
      - Companies
      - Companies
      - Applications
      - s
  /organizations/{org_name}/companies/{company_name}/apps/{app_name}:
    get:
      summary: Get Organizations Name Companies Company Name Apps App Name
      description: Gets the count    of API resources for a company app.
      operationId: getOrganizationsOrgNameCompaniesCompanyNameAppsAppName
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-name-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: query
        name: entity
        description: Mention entity as API resources
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: query
        description: Specify query value as count
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - ""
    post:
      summary: Post Organizations Name Companies Company Name Apps App Name
      description: Updates an existing company app.
      operationId: postOrganizationsOrgNameCompaniesCompanyNameAppsAppName
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-name-post
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
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
      - Companies
      - Companies
      - Applications
      - ""
    delete:
      summary: Delete Organizations Name Companies Company Name Apps App Name
      description: Deletes a company app.
      operationId: deleteOrganizationsOrgNameCompaniesCompanyNameAppsAppName
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-name-delete
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - ""
  /organizations/{org_name}/companies/{company_name}/apps/{app_name}/keys/{consumer_key}:
    get:
      summary: Get Organizations Name Companies Company Name Apps App Name Keys Consumer
        Key
      description: Gets the consumer key issued to a company app.
      operationId: getOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-get
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
    post:
      summary: Post Organizations Name Companies Company Name Apps App Name Keys Consumer
        Key
      description: Revokes the specific key of a company app.
      operationId: postOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-post
      parameters:
      - in: query
        name: action
        description: Mention action as revoke
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
    delete:
      summary: Delete Organizations Name Companies Company Name Apps App Name Keys
        Consumer Key
      description: Deletes a company app key.
      operationId: deleteOrganizationsOrgNameCompaniesCompanyNameAppsAppNameKeysConsumerKey
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-delete
      parameters:
      - in: path
        name: app_name
        description: Mention the app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: consumer_key
        description: Mention the consumer key
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - ""
      - Keys
      - Consumer
      - Key
  /organizations/{org_name}/companies/{company_name}/appfamilies:
    get:
      summary: Get Organizations Name Companies Company Name Appfamilies
      description: An expanded list of all app families in an organization, listing
        Apps in the collection.
      operationId: getOrganizationsOrgNameCompaniesCompanyNameAppfamilies
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappfamilies-get
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - Families
    post:
      summary: Post Organizations Name Companies Company Name Appfamilies
      description: Creates an app family.
      operationId: postOrganizationsOrgNameCompaniesCompanyNameAppfamilies
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappfamilies-post
      parameters:
      - in: path
        name: company_name
        description: Mention the company name
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
      - Companies
      - Companies
      - Applications
      - Families
  /organizations/{org_name}/companies/{company_name}/appfamilies/{appfamily_name}:
    get:
      summary: Get Organizations Name Companies Company Name Appfamilies Appfamily
        Name
      description: Gets a list of apps in an appfamily.
      operationId: getOrganizationsOrgNameCompaniesCompanyNameAppfamiliesAppfamilyName
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-get
      parameters:
      - in: path
        name: appfamily_name
        description: Mention app family name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - Families
      - Applications
      - family
    post:
      summary: Post Organizations Name Companies Company Name Appfamilies Appfamily
        Name
      description: Updates an existing app family.
      operationId: postOrganizationsOrgNameCompaniesCompanyNameAppfamiliesAppfamilyName
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-post
      parameters:
      - in: path
        name: appfamily_name
        description: Mention app family name
      - in: path
        name: company_name
        description: Mention the company name
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
      - Companies
      - Companies
      - Applications
      - Families
      - Applications
      - family
    delete:
      summary: Delete Organizations Name Companies Company Name Appfamilies Appfamily
        Name
      description: Deletes an App Family and all Apps it contains.
      operationId: deleteOrganizationsOrgNameCompaniesCompanyNameAppfamiliesAppfamilyName
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-delete
      parameters:
      - in: path
        name: appfamily_name
        description: Mention app family name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - Families
      - Applications
      - family
  /organizations/{org_name}/companies/{company_name}/appfamilies/{appfamily_name}/apps/{app_name}:
    delete:
      summary: Delete Organizations Name Companies Company Name Appfamilies Appfamily
        Name Apps App Name
      description: Removes an App from an App Family.
      operationId: deleteOrganizationsOrgNameCompaniesCompanyNameAppfamiliesAppfamilyNameAppsAppName
      x-api-path-slug: organizationsorg-namecompaniescompany-nameappfamiliesappfamily-nameappsapp-name-delete
      parameters:
      - in: path
        name: appfamily_name
        description: Mention app family name
      - in: path
        name: app_name
        description: Mention app name
      - in: path
        name: company_name
        description: Mention the company name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Companies
      - Companies
      - Applications
      - Families
      - Applications
      - family
      - Applications
      - ""
  /organizations/{org_name}/developers/{developer_email}/appfamilies:
    get:
      summary: Get Organizations Name Developers Developer Email Appfamilies
      description: An expanded list of all app families in an organization, listing
        Apps in the collection
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppfamilies
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappfamilies-get
      parameters:
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
      - Families
    post:
      summary: Post Organizations Name Developers Developer Email Appfamilies
      description: Creates an app family for developers.
      operationId: postOrganizationsOrgNameDevelopersDeveloperEmailAppfamilies
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappfamilies-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
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
      - Families
  /organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}:
    get:
      summary: Get Organizations Name Developers Developer Email Appfamilies Appfamily
        Name
      description: Gets a list of apps in an appfamily.
      operationId: getOrganizationsOrgNameDevelopersDeveloperEmailAppfamiliesAppfamilyName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-get
      parameters:
      - in: path
        name: appfamily_name
        description: Mention app family name
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
      - Families
      - Applications
      - family
    post:
      summary: Post Organizations Name Developers Developer Email Appfamilies Appfamily
        Name
      description: Updates an existing app family.
      operationId: postOrganizationsOrgNameDevelopersDeveloperEmailAppfamiliesAppfamilyName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-post
      parameters:
      - in: path
        name: appfamily_name
        description: Mention app family name
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
      - Families
      - Applications
      - family
    delete:
      summary: Delete Organizations Name Developers Developer Email Appfamilies Appfamily
        Name
      description: Deletes an App Family and all Apps it contains.
      operationId: deleteOrganizationsOrgNameDevelopersDeveloperEmailAppfamiliesAppfamilyName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-delete
      parameters:
      - in: path
        name: appfamily_name
        description: Mention app family name
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
      - Families
      - Applications
      - family
  /organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}/apps/{app_name}:
    delete:
      summary: Delete Organizations Name Developers Developer Email Appfamilies Appfamily
        Name Apps App Name
      description: Removes an App from an App Family.
      operationId: deleteOrganizationsOrgNameDevelopersDeveloperEmailAppfamiliesAppfamilyNameAppsAppName
      x-api-path-slug: organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-nameappsapp-name-delete
      parameters:
      - in: path
        name: appfamily_name
        description: Mention app family name
      - in: path
        name: app_name
        description: Mention app name
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
      - Families
      - Applications
      - family
      - Applications
      - ""
  /organizations/{org_name}/userroles:
    get:
      summary: Get Organizations Name Userroles
      description: Gets a list of roles available to users in an organization.
      operationId: getOrganizationsOrgNameUserroles
      x-api-path-slug: organizationsorg-nameuserroles-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
    post:
      summary: Post Organizations Name Userroles
      description: Creates a role in an organization.
      operationId: postOrganizationsOrgNameUserroles
      x-api-path-slug: organizationsorg-nameuserroles-post
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
      - Userroles
  /organizations/{org_name}/userroles/{role_name}:
    get:
      summary: Get Organizations Name Userroles Role Name
      description: Gets a role.
      operationId: getOrganizationsOrgNameUserrolesRoleName
      x-api-path-slug: organizationsorg-nameuserrolesrole-name-get
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
    delete:
      summary: Delete Organizations Name Userroles Role Name
      description: Deletes a role from an organization.
      operationId: deleteOrganizationsOrgNameUserrolesRoleName
      x-api-path-slug: organizationsorg-nameuserrolesrole-name-delete
      parameters:
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
  /organizations/{org_name}/resources:
    get:
      summary: Get Organizations Name Resources
      description: Gets a RBAC resource based on resource path.
      operationId: getOrganizationsOrgNameResources
      x-api-path-slug: organizationsorg-nameresources-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Resources
    post:
      summary: Post Organizations Name Resources
      description: Creates a resource.
      operationId: postOrganizationsOrgNameResources
      x-api-path-slug: organizationsorg-nameresources-post
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
      - Resources
    delete:
      summary: Delete Organizations Name Resources
      description: Deletes a resource.
      operationId: deleteOrganizationsOrgNameResources
      x-api-path-slug: organizationsorg-nameresources-delete
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Resources
  /organizations/{org_name}/userroles/{role_name}/permissions:
    get:
      summary: Get Organizations Name Userroles Role Name Permissions
      description: Gets a list of permissions associated with the specified resource
        for a single resource.
      operationId: getOrganizationsOrgNameUserrolesRoleNamePermissions
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissions-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
    post:
      summary: Post Organizations Name Userroles Role Name Permissions
      description: Associates permissions for a resource with a user role.
      operationId: postOrganizationsOrgNameUserrolesRoleNamePermissions
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissions-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
  /organizations/{org_name}/userroles/{role_name}/permissions/get:
    get:
      summary: Get Organizations Name Userroles Role Name Permissions Get
      description: Checks the particular userrole permission of a resource at organization
        level.
      operationId: getOrganizationsOrgNameUserrolesRoleNamePermissionsGet
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissionsget-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
      - Get
    delete:
      summary: Delete Organizations Name Userroles Role Name Permissions Get
      description: Deletes particular userrole permission at organization level.
      operationId: deleteOrganizationsOrgNameUserrolesRoleNamePermissionsGet
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissionsget-delete
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
      - Get
  /organizations/{org_name}/userroles/{role_name}/resourcepermissions:
    post:
      summary: Post Organizations Name Userroles Role Name Resourcepermissions
      description: Adds multiple resource permissions for resource at organization
        level.
      operationId: postOrganizationsOrgNameUserrolesRoleNameResourcepermissions
      x-api-path-slug: organizationsorg-nameuserrolesrole-nameresourcepermissions-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Resourcepermissions
---