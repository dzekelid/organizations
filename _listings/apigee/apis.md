---
name: Apigee
x-slug: apigee
description: Apigee Edge is a platform for developing and managing API proxies. Think
  of a proxy as an abstraction layer that fronts for your backend service APIs and
  provides value-added features like security, rate limiting, quotas, analytics, and
  more. The primary consumers of Edge API proxies are app developers who want to use
  your backend services.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Organizations
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/apis.md
specificationVersion: "0.14"
apis:
- name: Apigee Edge Get Organizations
  x-api-slug: apigee-edge
  description: Lists all the organizations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizations-get-openapi.md
- name: Apigee Edge Post Organizations
  x-api-slug: apigee-edge
  description: Creates an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizations-post-openapi.md
- name: Apigee Edge Get Organizations Name
  x-api-slug: apigee-edge
  description: Gets a specific organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-name-get-openapi.md
- name: Apigee Edge Put Organizations Name
  x-api-slug: apigee-edge
  description: Updates the description of a specific organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-name-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-name-put-openapi.md
- name: Apigee Edge Delete Organizations Name
  x-api-slug: apigee-edge
  description: Deletes a specific organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Deployments
  x-api-slug: apigee-edge
  description: Gets all deployments of an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/deployments
  tags: Organizations,Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedeployments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedeployments-get-openapi.md
- name: Apigee Edge Get Organizations Name Pods
  x-api-slug: apigee-edge
  description: Gets all the pods associated with an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/pods
  tags: Organizations,Pods
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namepods-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namepods-get-openapi.md
- name: Apigee Edge Post Organizations Name Pods
  x-api-slug: apigee-edge
  description: Disassociates a pod from an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/pods
  tags: Organizations,Pods
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namepods-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namepods-post-openapi.md
- name: Apigee Edge Get Organizations Name Environments
  x-api-slug: apigee-edge
  description: Lists all the environments in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments
  tags: Organizations,Environments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironments-get-openapi.md
- name: Apigee Edge Post Organizations Name Environments
  x-api-slug: apigee-edge
  description: Creates an environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments
  tags: Organizations,Environments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironments-post-openapi.md
- name: Apigee Edge Get Organizations Name Environments Env Name
  x-api-slug: apigee-edge
  description: Gets details for an environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}
  tags: Organizations,Environments,Env
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-name-get-openapi.md
- name: Apigee Edge Post Organizations Name Environments Env Name
  x-api-slug: apigee-edge
  description: Updates an environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}
  tags: Organizations,Environments,Env
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Environments Env Name
  x-api-slug: apigee-edge
  description: Deletes a specific environment in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}
  tags: Organizations,Environments,Env
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Environments Env Name Deployments
  x-api-slug: apigee-edge
  description: Gets the deployments for an environment in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/deployments
  tags: Organizations,Environments,Env,Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namedeployments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namedeployments-get-openapi.md
- name: Apigee Edge Get Organizations Name Environments Env Name API Name Deployments
  x-api-slug: apigee-edge
  description: Gets the deployments for an API Proxy in the given environment in an
    organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/apis/{api_name}/deployments
  tags: Organizations,Environments,Envs,APIs,Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameapisapi-namedeployments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameapisapi-namedeployments-get-openapi.md
- name: Apigee Edge Get Organizations Name Environments Env Name API Name Revisions
    Revision Number Deployments
  x-api-slug: apigee-edge
  description: "Gets the deployments for an API Proxy\xE2\x80\x99s revision for an
    environment in an organization."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/apis/{api_name}/revisions/{revision_number}/deployments
  tags: Organizations,Environments,Envs,APIs,Revisions,Revision,Number,Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameapisapi-namerevisionsrevision-numberdeployments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameapisapi-namerevisionsrevision-numberdeployments-get-openapi.md
- name: Apigee Edge Get Organizations Name Environments Env Name Servers
  x-api-slug: apigee-edge
  description: Gets the servers that are bound to an environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/servers
  tags: Organizations,Environments,Env,Servers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameservers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameservers-get-openapi.md
- name: Apigee Edge Post Organizations Name Environments Env Name Servers
  x-api-slug: apigee-edge
  description: Add servers into the environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/servers
  tags: Organizations,Environments,Env,Servers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameservers-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameservers-post-openapi.md
- name: Apigee Edge Delete Organizations Name Environments Env Name Servers
  x-api-slug: apigee-edge
  description: Deletes servers from the environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/servers
  tags: Organizations,Environments,Env,Servers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameservers-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-nameservers-delete-openapi.md
- name: Apigee Edge Get Organizations Name Environments Env Name Virtualhosts
  x-api-slug: apigee-edge
  description: Lists all virtual hosts in an environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/virtualhosts
  tags: Organizations,Environments,Env,Virtualhosts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhosts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhosts-get-openapi.md
- name: Apigee Edge Post Organizations Name Environments Env Name Virtualhosts
  x-api-slug: apigee-edge
  description: Creates a virtual host.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/virtualhosts
  tags: Organizations,Environments,Env,Virtualhosts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhosts-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhosts-post-openapi.md
- name: Apigee Edge Get Organizations Name Environments Env Name Virtualhosts Virtualhost
    Name
  x-api-slug: apigee-edge
  description: Gets details for a named virtual host .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/virtualhosts/{virtualhost_name}
  tags: Organizations,Environments,Env,Virtualhosts,Virtualhost
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-get-openapi.md
- name: Apigee Edge Post Organizations Name Environments Env Name Virtualhosts Virtualhost
    Name
  x-api-slug: apigee-edge
  description: Updates a specific virtual host in an environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/virtualhosts/{virtualhost_name}
  tags: Organizations,Environments,Env,Virtualhosts,Virtualhost
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Environments Env Name Virtualhosts Virtualhost
    Name
  x-api-slug: apigee-edge
  description: Deletes a specific virtual host in an environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/environments/{env_name}/virtualhosts/{virtualhost_name}
  tags: Organizations,Environments,Env,Virtualhosts,Virtualhost
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameenvironmentsenv-namevirtualhostsvirtualhost-name-delete-openapi.md
- name: Apigee Edge Post Organizations Name API Name Revisions Revision Number Deployments
  x-api-slug: apigee-edge
  description: Undeploys an API proxy revision from an environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis/{api_name}/revisions/{revision_number}/deployments
  tags: Organizationss,APIs,Revisions,Revision,Number,Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-numberdeployments-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-numberdeployments-post-openapi.md
- name: Apigee Edge Get Organizations Name APIs
  x-api-slug: apigee-edge
  description: Gets all APIs in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis
  tags: Organizations,APIs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapis-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapis-get-openapi.md
- name: Apigee Edge Post Organizations Name APIs
  x-api-slug: apigee-edge
  description: Uploads a ZIP-formatted API proxy configuration bundle from a local
    machine to an organization on the API Platform.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis
  tags: Organizations,APIs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapis-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapis-post-openapi.md
- name: Apigee Edge Get Organizations Name API Name
  x-api-slug: apigee-edge
  description: Gets an API proxy by name, providing a list of existing revisions of
    the API proxy configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis/{api_name}
  tags: Organizationss,APIs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-name-get-openapi.md
- name: Apigee Edge Delete Organizations Name API Name
  x-api-slug: apigee-edge
  description: Deletes an API and all associated endpoints, policies, resources, and
    revisions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis/{api_name}
  tags: Organizationss,APIs
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-name-delete-openapi.md
- name: Apigee Edge Put Organizations Name API Name Revisions Revision Number
  x-api-slug: apigee-edge
  description: Use the POST method to update a specific API proxy in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis/{api_name}/revisions/revision_number
  tags: Organizationss,APIs,Revisions,Revision,Number
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-number-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-number-put-openapi.md
- name: Apigee Edge Get Organizations Name API Name Revisions Revision Number
  x-api-slug: apigee-edge
  description: Exports an API from Apigee to the local machine a ZIP bundle of config
    and code files..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis/{api_name}/revisions/{revision_number}
  tags: Organizationss,APIs,Revisions,Revision,Number
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-number-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-number-get-openapi.md
- name: Apigee Edge Delete Organizations Name API Name Revisions Revision Number
  x-api-slug: apigee-edge
  description: Deletes a specific revision of an API.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis/{api_name}/revisions/{revision_number}
  tags: Organizationss,APIs,Revisions,Revision,Number
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-number-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-number-delete-openapi.md
- name: Apigee Edge Get Organizations Name API Name Deployments
  x-api-slug: apigee-edge
  description: Returns detail on deployments of the API specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis/{api_name}/deployments
  tags: Organizationss,APIs,Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namedeployments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namedeployments-get-openapi.md
- name: Apigee Edge Get Organizations Name API Name Revisions Revision Name Deployments
  x-api-slug: apigee-edge
  description: Get deployments for a revision of an API proxy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apis/{api_name}/revisions/{revision_name}/deployments
  tags: Organizationss,APIs,Revisions,Revision,Deployments
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-namedeployments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapisapi-namerevisionsrevision-namedeployments-get-openapi.md
- name: Apigee Edge Get Organizations Name Apiproducts
  x-api-slug: apigee-edge
  description: Lists all API products by name for an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apiproducts
  tags: Organizations,API,Products
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproducts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproducts-get-openapi.md
- name: Apigee Edge Post Organizations Name Apiproducts
  x-api-slug: apigee-edge
  description: 'Create an API product: a list of API resources combined with Quota
    settings that you can use to deliver customized API bundles to your developers.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apiproducts
  tags: Organizations,API,Products
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproducts-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproducts-post-openapi.md
- name: Apigee Edge Get Organizations Name Apiproducts Apiproduct Name
  x-api-slug: apigee-edge
  description: Gets the list of keys/apps/developers for an API product of an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apiproducts/{apiproduct_name}
  tags: Organizations,API,Products,API,Productss
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproductsapiproduct-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproductsapiproduct-name-get-openapi.md
- name: Apigee Edge Put Organizations Name Apiproducts Apiproduct Name
  x-api-slug: apigee-edge
  description: This method updates an existing API product.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apiproducts/{apiproduct_name}
  tags: Organizations,API,Products,API,Productss
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproductsapiproduct-name-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproductsapiproduct-name-put-openapi.md
- name: Apigee Edge Delete Organizations Name Apiproducts Apiproduct Name
  x-api-slug: apigee-edge
  description: Deletes an API product.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/apiproducts/{apiproduct_name}
  tags: Organizations,API,Products,API,Productss
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproductsapiproduct-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameapiproductsapiproduct-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Developers
  x-api-slug: apigee-edge
  description: Gets the developer profile by registered date.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers
  tags: Organizations,Developers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopers-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers
  x-api-slug: apigee-edge
  description: Create a developer in an organization .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers
  tags: Organizations,Developers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopers-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopers-post-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Name
  x-api-slug: apigee-edge
  description: Get a count of apps by developer email address.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_name}
  tags: Organizations,Developers,Developer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-name-get-openapi.md
- name: Apigee Edge Put Organizations Name Developers Developer Name
  x-api-slug: apigee-edge
  description: Update an existing developer profile with new values or additional
    attributes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_name}
  tags: Organizations,Developers,Developer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-name-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-name-put-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Name
  x-api-slug: apigee-edge
  description: Sets the status of a developer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_name}
  tags: Organizations,Developers,Developer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Name
  x-api-slug: apigee-edge
  description: Deletes a developer from an Organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_name}
  tags: Organizations,Developers,Developer
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps
  x-api-slug: apigee-edge
  description: Provides an expanded view of a developer's collection of apps .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps
  tags: Organizations,Developers,Developer,Email,Applications,s
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailapps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailapps-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Apps
  x-api-slug: apigee-edge
  description: Creates an app associated with a developer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps
  tags: Organizations,Developers,Developer,Email,Applications,s
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailapps-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailapps-post-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
  x-api-slug: apigee-edge
  description: Gets a count of all API resources in the API products accessible by
    a developer app .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-get-openapi.md
- name: Apigee Edge Put Organizations Name Developers Developer Email Apps App Name
  x-api-slug: apigee-edge
  description: Updates the app to get a new set of consumer credentials.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-put-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Apps App Name
  x-api-slug: apigee-edge
  description: Revokes a Developer App, disabling access to all API Products .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Apps App
    Name
  x-api-slug: apigee-edge
  description: Delete a Developer's App.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key
  x-api-slug: apigee-edge
  description: Returns details for a consumer key for a developer app .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key
  x-api-slug: apigee-edge
  description: Revokes a developer app key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Apps App
    Name Keys Consumer Key
  x-api-slug: apigee-edge
  description: Deletes a consumer key that belongs to an app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-key-delete-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key Apiproducts Apiproduct Name
  x-api-slug: apigee-edge
  description: Revokes the association of an API Product with a Developer App's consumer
    key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/apiproducts/{apiproduct_name}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key,API,Products,API,Productss
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Apps App
    Name Keys Consumer Key Apiproducts Apiproduct Name
  x-api-slug: apigee-edge
  description: Removes an API product from a developer app key profile, and thereby
    renders the developer app unable to access the URIs defined in the API product
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/apiproducts/{apiproduct_name}
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key,API,Products,API,Productss
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyapiproductsapiproduct-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Oauth1accesstokens
  x-api-slug: apigee-edge
  description: Get count of OAuth 1.0 access tokens for a developer's app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/oauth1accesstokens
  tags: Organizations,Developers,Developer,Email,Applications,,Oauth1accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth1accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth1accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Oauth2accesstokens
  x-api-slug: apigee-edge
  description: Get count of    OAuth 2.0 access tokens for a developer's app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/oauth2accesstokens
  tags: Organizations,Developers,Developer,Email,Applications,,Oauth2accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth2accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-nameoauth2accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key Oauth1accesstokens
  x-api-slug: apigee-edge
  description: Get count of OAuth 1.0 access tokens for a developer's app key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth1accesstokens
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key,Oauth1accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth1accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth1accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Apps App Name
    Keys Consumer Key Oauth2accesstokens
  x-api-slug: apigee-edge
  description: Get count of OAuth 2.0 access tokens for a developer's app key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/apps/{app_name}/keys/{consumer_key}/oauth2accesstokens
  tags: Organizations,Developers,Developer,Email,Applications,,Keys,Consumer,Key,Oauth2accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth2accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappsapp-namekeysconsumer-keyoauth2accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Oauth1 Requesttokens Request Token
  x-api-slug: apigee-edge
  description: Gets the Oauth 1.0 a request token for the speficied consumer key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/requesttokens/{request_token}
  tags: Organizations,Oauth1,Requesttokens,Request,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1requesttokensrequest-token-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1requesttokensrequest-token-get-openapi.md
- name: Apigee Edge Post Organizations Name Oauth1 Requesttokens Request Token
  x-api-slug: apigee-edge
  description: Revokes an OAuth 1.0 a request token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/requesttokens/{request_token}
  tags: Organizations,Oauth1,Requesttokens,Request,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1requesttokensrequest-token-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1requesttokensrequest-token-post-openapi.md
- name: Apigee Edge Delete Organizations Name Oauth1 Requesttokens Request Token
  x-api-slug: apigee-edge
  description: Deletes the request token specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/requesttokens/{request_token}
  tags: Organizations,Oauth1,Requesttokens,Request,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1requesttokensrequest-token-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1requesttokensrequest-token-delete-openapi.md
- name: Apigee Edge Get Organizations Name Oauth1 Requesttokens
  x-api-slug: apigee-edge
  description: Returns list of all OAuth 1.0a request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/requesttokens
  tags: Organizations,Oauth1,Requesttokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1requesttokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1requesttokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Oauth1 Verifiers Verifier Code
  x-api-slug: apigee-edge
  description: Gets the detail of given verifier code.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/verifiers/{verifier_code}
  tags: Organizations,Oauth1,Verifiers,Verifier,Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1verifiersverifier-code-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1verifiersverifier-code-get-openapi.md
- name: Apigee Edge Delete Organizations Name Oauth1 Verifiers Verifier Code
  x-api-slug: apigee-edge
  description: Deletes the specified verifier code, which is the verifier code given
    by the provider.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/verifiers/{verifier_code}
  tags: Organizations,Oauth1,Verifiers,Verifier,Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1verifiersverifier-code-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1verifiersverifier-code-delete-openapi.md
- name: Apigee Edge Get Organizations Name Oauth1 Verifiers
  x-api-slug: apigee-edge
  description: Gets a list of all verifiers and details for each verifier in an Organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/verifiers
  tags: Organizations,Oauth1,Verifiers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1verifiers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1verifiers-get-openapi.md
- name: Apigee Edge Get Organizations Name Oauth1 Accesstokens Access Token
  x-api-slug: apigee-edge
  description: Fetches the details of given access token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/accesstokens/{access_token}
  tags: Organizations,Oauth1,Accesstokens,Access,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1accesstokensaccess-token-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1accesstokensaccess-token-get-openapi.md
- name: Apigee Edge Post Organizations Name Oauth1 Accesstokens Access Token
  x-api-slug: apigee-edge
  description: Revokes the specified access token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/accesstokens/{access_token}
  tags: Organizations,Oauth1,Accesstokens,Access,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1accesstokensaccess-token-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1accesstokensaccess-token-post-openapi.md
- name: Apigee Edge Delete Organizations Name Oauth1 Accesstokens Access Token
  x-api-slug: apigee-edge
  description: Deletes the specified access token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/accesstokens/{access_token}
  tags: Organizations,Oauth1,Accesstokens,Access,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1accesstokensaccess-token-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1accesstokensaccess-token-delete-openapi.md
- name: Apigee Edge Get Organizations Name Oauth1 Accesstokens
  x-api-slug: apigee-edge
  description: Returns a count of all 1.0a access tokens in an orgnization .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth1/accesstokens
  tags: Organizations,Oauth1,Accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth1accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Oauth2 Authorizationcodes Authorization
    Code
  x-api-slug: apigee-edge
  description: Get a specific Authorization Code.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth2/authorizationcodes/{authorization_code}
  tags: Organizations,Oauth2,Authorizationcodes,Authorization,Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2authorizationcodesauthorization-code-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2authorizationcodesauthorization-code-get-openapi.md
- name: Apigee Edge Delete Organizations Name Oauth2 Authorizationcodes Authorization
    Code
  x-api-slug: apigee-edge
  description: Deletes the given authorization Code.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth2/authorizationcodes/{authorization_code}
  tags: Organizations,Oauth2,Authorizationcodes,Authorization,Code
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2authorizationcodesauthorization-code-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2authorizationcodesauthorization-code-delete-openapi.md
- name: Apigee Edge Get Organizations Name Oauth2 Authorizationcodes
  x-api-slug: apigee-edge
  description: Lists all authorization codes in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth2/authorizationcodes
  tags: Organizations,Oauth2,Authorizationcodes
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2authorizationcodes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2authorizationcodes-get-openapi.md
- name: Apigee Edge Get Organizations Name Oauth2 Accesstokens Access Token
  x-api-slug: apigee-edge
  description: Gets details of a specific access token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth2/accesstokens/{access_token}
  tags: Organizations,Oauth2,Accesstokens,Access,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2accesstokensaccess-token-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2accesstokensaccess-token-get-openapi.md
- name: Apigee Edge Post Organizations Name Oauth2 Accesstokens Access Token
  x-api-slug: apigee-edge
  description: Revokes a specific access token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth2/accesstokens/{access_token}
  tags: Organizations,Oauth2,Accesstokens,Access,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2accesstokensaccess-token-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2accesstokensaccess-token-post-openapi.md
- name: Apigee Edge Delete Organizations Name Oauth2 Accesstokens Access Token
  x-api-slug: apigee-edge
  description: Deletes a specific access token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth2/accesstokens/{access_token}
  tags: Organizations,Oauth2,Accesstokens,Access,Token
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2accesstokensaccess-token-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2accesstokensaccess-token-delete-openapi.md
- name: Apigee Edge Get Organizations Name Oauth2 Accesstokens
  x-api-slug: apigee-edge
  description: Get count of OAuth 2.0 access tokens under an organization .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/oauth2/accesstokens
  tags: Organizations,Oauth2,Accesstokens
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2accesstokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameoauth2accesstokens-get-openapi.md
- name: Apigee Edge Get Organizations Name Keyvaluemaps
  x-api-slug: apigee-edge
  description: Returns an expanded view of all Maps scoped by organization, environment
    or API.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/keyvaluemaps
  tags: Organizations,Keyvaluemaps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemaps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemaps-get-openapi.md
- name: Apigee Edge Post Organizations Name Keyvaluemaps
  x-api-slug: apigee-edge
  description: Creates a KeyValueMap.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/keyvaluemaps
  tags: Organizations,Keyvaluemaps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemaps-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemaps-post-openapi.md
- name: Apigee Edge Get Organizations Name Keyvaluemaps Map Name Entries Entry Name
  x-api-slug: apigee-edge
  description: Gets a specific entry details.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/keyvaluemaps/{map_name}/entries/{entry_name}
  tags: Organizations,Keyvaluemaps,Map,Entries,Entry
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-nameentriesentry-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-nameentriesentry-name-get-openapi.md
- name: Apigee Edge Delete Organizations Name Keyvaluemaps Map Name Entries Entry
    Name
  x-api-slug: apigee-edge
  description: Deletes a single entry by name.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/keyvaluemaps/{map_name}/entries/{entry_name}
  tags: Organizations,Keyvaluemaps,Map,Entries,Entry
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-nameentriesentry-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-nameentriesentry-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Keyvaluemaps Map Name
  x-api-slug: apigee-edge
  description: Gets a KeyValueMap by name, along with associated entries.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/keyvaluemaps/{map_name}
  tags: Organizations,Keyvaluemaps,Map
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-name-get-openapi.md
- name: Apigee Edge Put Organizations Name Keyvaluemaps Map Name
  x-api-slug: apigee-edge
  description: Updates an existing KeyValueMap.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/keyvaluemaps/{map_name}
  tags: Organizations,Keyvaluemaps,Map
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-name-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-name-put-openapi.md
- name: Apigee Edge Delete Organizations Name Keyvaluemaps Map Name
  x-api-slug: apigee-edge
  description: Deletes a KeyValueMap and all associated entries.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/keyvaluemaps/{map_name}
  tags: Organizations,Keyvaluemaps,Map
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namekeyvaluemapsmap-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Companies
  x-api-slug: apigee-edge
  description: Returns an expanded list of companies, displaying a full profile for
    each company in the organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies
  tags: Organizations,Companies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompanies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompanies-get-openapi.md
- name: Apigee Edge Post Organizations Name Companies
  x-api-slug: apigee-edge
  description: Creates a company in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies
  tags: Organizations,Companies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompanies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompanies-post-openapi.md
- name: Apigee Edge Get Organizations Name Companies Company Name
  x-api-slug: apigee-edge
  description: Gets details for a Company.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}
  tags: Organizations,Companies,Companies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-name-get-openapi.md
- name: Apigee Edge Put Organizations Name Companies Company Name
  x-api-slug: apigee-edge
  description: Updates an existing Company.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}
  tags: Organizations,Companies,Companies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-name-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-name-put-openapi.md
- name: Apigee Edge Delete Organizations Name Companies Company Name
  x-api-slug: apigee-edge
  description: Deletes an existing Company.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}
  tags: Organizations,Companies,Companies
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Companies Company Name Developers
  x-api-slug: apigee-edge
  description: Lists all developers associated with a company.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/developers
  tags: Organizations,Companies,Companies,Developers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-namedevelopers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-namedevelopers-get-openapi.md
- name: Apigee Edge Post Organizations Name Companies Company Name Developers
  x-api-slug: apigee-edge
  description: Adds a developer to a company.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/developers
  tags: Organizations,Companies,Companies,Developers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-namedevelopers-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-namedevelopers-post-openapi.md
- name: Apigee Edge Delete Organizations Name Companies Company Name Developers Developer
    Email
  x-api-slug: apigee-edge
  description: Removes the association of a Developer with a Company.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/developers/{developer_email}
  tags: Organizations,Companies,Companies,Developers,Developer,Email
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-namedevelopersdeveloper-email-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-namedevelopersdeveloper-email-delete-openapi.md
- name: Apigee Edge Get Organizations Name Companies Company Name Apps
  x-api-slug: apigee-edge
  description: Gets an expanded list company apps .
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/apps
  tags: Organizations,Companies,Companies,Applications,s
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameapps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameapps-get-openapi.md
- name: Apigee Edge Post Organizations Name Companies Company Name Apps
  x-api-slug: apigee-edge
  description: Creates an app for a company.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/apps
  tags: Organizations,Companies,Companies,Applications,s
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameapps-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameapps-post-openapi.md
- name: Apigee Edge Get Organizations Name Companies Company Name Apps App Name
  x-api-slug: apigee-edge
  description: Gets the count    of API resources for a company app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/apps/{app_name}
  tags: Organizations,Companies,Companies,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-name-get-openapi.md
- name: Apigee Edge Post Organizations Name Companies Company Name Apps App Name
  x-api-slug: apigee-edge
  description: Updates an existing company app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/apps/{app_name}
  tags: Organizations,Companies,Companies,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Companies Company Name Apps App Name
  x-api-slug: apigee-edge
  description: Deletes a company app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/apps/{app_name}
  tags: Organizations,Companies,Companies,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Companies Company Name Apps App Name Keys
    Consumer Key
  x-api-slug: apigee-edge
  description: Gets the consumer key issued to a company app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Companies,Companies,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-get-openapi.md
- name: Apigee Edge Post Organizations Name Companies Company Name Apps App Name Keys
    Consumer Key
  x-api-slug: apigee-edge
  description: Revokes the specific key of a company app.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Companies,Companies,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-post-openapi.md
- name: Apigee Edge Delete Organizations Name Companies Company Name Apps App Name
    Keys Consumer Key
  x-api-slug: apigee-edge
  description: Deletes a company app key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/apps/{app_name}/keys/{consumer_key}
  tags: Organizations,Companies,Companies,Applications,,Keys,Consumer,Key
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappsapp-namekeysconsumer-key-delete-openapi.md
- name: Apigee Edge Get Organizations Name Companies Company Name Appfamilies
  x-api-slug: apigee-edge
  description: An expanded list of all app families in an organization, listing Apps
    in the collection.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/appfamilies
  tags: Organizations,Companies,Companies,Applications,Families
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamilies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamilies-get-openapi.md
- name: Apigee Edge Post Organizations Name Companies Company Name Appfamilies
  x-api-slug: apigee-edge
  description: Creates an app family.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/appfamilies
  tags: Organizations,Companies,Companies,Applications,Families
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamilies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamilies-post-openapi.md
- name: Apigee Edge Get Organizations Name Companies Company Name Appfamilies Appfamily
    Name
  x-api-slug: apigee-edge
  description: Gets a list of apps in an appfamily.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/appfamilies/{appfamily_name}
  tags: Organizations,Companies,Companies,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-get-openapi.md
- name: Apigee Edge Post Organizations Name Companies Company Name Appfamilies Appfamily
    Name
  x-api-slug: apigee-edge
  description: Updates an existing app family.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/appfamilies/{appfamily_name}
  tags: Organizations,Companies,Companies,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Companies Company Name Appfamilies Appfamily
    Name
  x-api-slug: apigee-edge
  description: Deletes an App Family and all Apps it contains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/appfamilies/{appfamily_name}
  tags: Organizations,Companies,Companies,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamiliesappfamily-name-delete-openapi.md
- name: Apigee Edge Delete Organizations Name Companies Company Name Appfamilies Appfamily
    Name Apps App Name
  x-api-slug: apigee-edge
  description: Removes an App from an App Family.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/companies/{company_name}/appfamilies/{appfamily_name}/apps/{app_name}
  tags: Organizations,Companies,Companies,Applications,Families,Applications,family,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamiliesappfamily-nameappsapp-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namecompaniescompany-nameappfamiliesappfamily-nameappsapp-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Appfamilies
  x-api-slug: apigee-edge
  description: An expanded list of all app families in an organization, listing Apps
    in the collection
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies
  tags: Organizations,Developers,Developer,Email,Applications,Families
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamilies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamilies-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Appfamilies
  x-api-slug: apigee-edge
  description: Creates an app family for developers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies
  tags: Organizations,Developers,Developer,Email,Applications,Families
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamilies-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamilies-post-openapi.md
- name: Apigee Edge Get Organizations Name Developers Developer Email Appfamilies
    Appfamily Name
  x-api-slug: apigee-edge
  description: Gets a list of apps in an appfamily.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}
  tags: Organizations,Developers,Developer,Email,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-get-openapi.md
- name: Apigee Edge Post Organizations Name Developers Developer Email Appfamilies
    Appfamily Name
  x-api-slug: apigee-edge
  description: Updates an existing app family.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}
  tags: Organizations,Developers,Developer,Email,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-post-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Appfamilies
    Appfamily Name
  x-api-slug: apigee-edge
  description: Deletes an App Family and all Apps it contains.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}
  tags: Organizations,Developers,Developer,Email,Applications,Families,Applications,family
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-name-delete-openapi.md
- name: Apigee Edge Delete Organizations Name Developers Developer Email Appfamilies
    Appfamily Name Apps App Name
  x-api-slug: apigee-edge
  description: Removes an App from an App Family.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/developers/{developer_email}/appfamilies/{appfamily_name}/apps/{app_name}
  tags: Organizations,Developers,Developer,Email,Applications,Families,Applications,family,Applications,
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-nameappsapp-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-namedevelopersdeveloper-emailappfamiliesappfamily-nameappsapp-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Userroles
  x-api-slug: apigee-edge
  description: Gets a list of roles available to users in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles
  tags: Organizations,Userroles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserroles-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserroles-get-openapi.md
- name: Apigee Edge Post Organizations Name Userroles
  x-api-slug: apigee-edge
  description: Creates a role in an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles
  tags: Organizations,Userroles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserroles-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserroles-post-openapi.md
- name: Apigee Edge Get Organizations Name Userroles Role Name
  x-api-slug: apigee-edge
  description: Gets a role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles/{role_name}
  tags: Organizations,Userroles,Role
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-name-get-openapi.md
- name: Apigee Edge Delete Organizations Name Userroles Role Name
  x-api-slug: apigee-edge
  description: Deletes a role from an organization.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles/{role_name}
  tags: Organizations,Userroles,Role
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-name-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-name-delete-openapi.md
- name: Apigee Edge Get Organizations Name Resources
  x-api-slug: apigee-edge
  description: Gets a RBAC resource based on resource path.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/resources
  tags: Organizations,Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameresources-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameresources-get-openapi.md
- name: Apigee Edge Post Organizations Name Resources
  x-api-slug: apigee-edge
  description: Creates a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/resources
  tags: Organizations,Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameresources-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameresources-post-openapi.md
- name: Apigee Edge Delete Organizations Name Resources
  x-api-slug: apigee-edge
  description: Deletes a resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/resources
  tags: Organizations,Resources
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameresources-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameresources-delete-openapi.md
- name: Apigee Edge Get Organizations Name Userroles Role Name Permissions
  x-api-slug: apigee-edge
  description: Gets a list of permissions associated with the specified resource for
    a single resource.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles/{role_name}/permissions
  tags: Organizations,Userroles,Role,Permissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-namepermissions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-namepermissions-get-openapi.md
- name: Apigee Edge Post Organizations Name Userroles Role Name Permissions
  x-api-slug: apigee-edge
  description: Associates permissions for a resource with a user role.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles/{role_name}/permissions
  tags: Organizations,Userroles,Role,Permissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-namepermissions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-namepermissions-post-openapi.md
- name: Apigee Edge Get Organizations Name Userroles Role Name Permissions Get
  x-api-slug: apigee-edge
  description: Checks the particular userrole permission of a resource at organization
    level.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles/{role_name}/permissions/get
  tags: Organizations,Userroles,Role,Permissions,Get
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-namepermissionsget-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-namepermissionsget-get-openapi.md
- name: Apigee Edge Delete Organizations Name Userroles Role Name Permissions Get
  x-api-slug: apigee-edge
  description: Deletes particular userrole permission at organization level.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles/{role_name}/permissions/get
  tags: Organizations,Userroles,Role,Permissions,Get
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-namepermissionsget-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-namepermissionsget-delete-openapi.md
- name: Apigee Edge Post Organizations Name Userroles Role Name Resourcepermissions
  x-api-slug: apigee-edge
  description: Adds multiple resource permissions for resource at organization level.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1///organizations/{org_name}/userroles/{role_name}/resourcepermissions
  tags: Organizations,Userroles,Role,Resourcepermissions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-nameresourcepermissions-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/organizationsorg-nameuserrolesrole-nameresourcepermissions-post-openapi.md
- name: Apigee Edge
  x-api-slug: apigee-edge
  description: Apigee Edge is a platform for developing and managing API proxies.
    Think of a proxy as an abstraction layer that fronts for your backend service
    APIs and provides value-added features like security, rate limiting, quotas, analytics,
    and more. The primary consumers of Edge API proxies are app developers who want
    to use your backend services.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/apigee-edge.png
  humanURL: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
  baseURL: https://api.enterprise.apigee.com//v1/
  tags: Organizations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/apigee/openapi.md
x-common:
- type: x-website
  url: https://docs.apigee.com/api-platform/get-started/what-apigee-edge
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---