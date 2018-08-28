---
name: Google Cloud Resource Manager
x-slug: google-cloud-resource-manager
description: Google Cloud Platform provides resource containers such as Organizations
  and Projects, that allow you to group and hierarchically organize other Cloud Platform
  resources. This hierarchical organization lets you easily manage common aspects
  of your resources such as access control and configuration settings. The Google
  Cloud Resource Manager service enables you to programmatically manage these resource
  containers.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Organizations
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Google Cloud Resource Manager - Search Organization
  x-api-slug: v1organizationssearch-post
  description: |-
    Searches Organization resources that are visible to the user and satisfy
    the specified filter. This method returns Organizations in an unspecified
    order. New Organizations do not necessarily appear at the end of the
    results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1organizationssearch-post-openapi.md
- name: Google Cloud Resource Manager - Get Organization IAM Policy
  x-api-slug: v1resourcegetiampolicy-post
  description: |-
    Gets the access control policy for an Organization resource. May be empty
    if no such policy or resource exists. The `resource` field should be the
    organization's resource name, e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcegetiampolicy-post-openapi.md
- name: Google Cloud Resource Manager - Set Organization IAM Policy
  x-api-slug: v1resourcesetiampolicy-post
  description: |-
    Sets the access control policy on an Organization resource. Replaces any
    existing policy. The `resource` field should be the organization's resource
    name, e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcesetiampolicy-post-openapi.md
- name: Google Cloud Resource Manager - TEst Organization IAM Permissions
  x-api-slug: v1resourcetestiampermissions-post
  description: |-
    Returns permissions that a caller has on the specified Organization.
    The `resource` field should be the organization's resource name,
    e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcetestiampermissions-post-openapi.md
- name: Google Cloud Resource Manager - Search Organization
  x-api-slug: v1organizationssearch-post
  description: |-
    Searches Organization resources that are visible to the user and satisfy
    the specified filter. This method returns Organizations in an unspecified
    order. New Organizations do not necessarily appear at the end of the
    results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1organizationssearch-post-openapi.md
- name: Google Cloud Resource Manager - Get Organization IAM Policy
  x-api-slug: v1resourcegetiampolicy-post
  description: |-
    Gets the access control policy for an Organization resource. May be empty
    if no such policy or resource exists. The `resource` field should be the
    organization's resource name, e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcegetiampolicy-post-openapi.md
- name: Google Cloud Resource Manager - Set Organization IAM Policy
  x-api-slug: v1resourcesetiampolicy-post
  description: |-
    Sets the access control policy on an Organization resource. Replaces any
    existing policy. The `resource` field should be the organization's resource
    name, e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcesetiampolicy-post-openapi.md
- name: Google Cloud Resource Manager - TEst Organization IAM Permissions
  x-api-slug: v1resourcetestiampermissions-post
  description: |-
    Returns permissions that a caller has on the specified Organization.
    The `resource` field should be the organization's resource name,
    e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcetestiampermissions-post-openapi.md
- name: Google Cloud Resource Manager - Search Organization
  x-api-slug: v1organizationssearch-post
  description: |-
    Searches Organization resources that are visible to the user and satisfy
    the specified filter. This method returns Organizations in an unspecified
    order. New Organizations do not necessarily appear at the end of the
    results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1organizationssearch-post-openapi.md
- name: Google Cloud Resource Manager - Get Organization IAM Policy
  x-api-slug: v1resourcegetiampolicy-post
  description: |-
    Gets the access control policy for an Organization resource. May be empty
    if no such policy or resource exists. The `resource` field should be the
    organization's resource name, e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcegetiampolicy-post-openapi.md
- name: Google Cloud Resource Manager - Set Organization IAM Policy
  x-api-slug: v1resourcesetiampolicy-post
  description: |-
    Sets the access control policy on an Organization resource. Replaces any
    existing policy. The `resource` field should be the organization's resource
    name, e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcesetiampolicy-post-openapi.md
- name: Google Cloud Resource Manager - TEst Organization IAM Permissions
  x-api-slug: v1resourcetestiampermissions-post
  description: |-
    Returns permissions that a caller has on the specified Organization.
    The `resource` field should be the organization's resource name,
    e.g. "organizations/123".
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Generic-GCP.png
  humanURL: https://cloud.google.com/resource-manager/
  baseURL: ://cloudresourcemanager.googleapis.com//
  tags: Orchestration, Google APIs, Management, Stack Network, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/google-cloud-resource-manager/v1resourcetestiampermissions-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.cloud.pub.sub.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.cloud.resource.manager.stack.network
- type: x-authentication
  url: https://cloud.google.com/resource-manager/docs/authorizing
- type: x-code
  url: https://cloud.google.com/resource-manager/docs/libraries
- type: x-documentation
  url: https://cloud.google.com/resource-manager/docs/
- type: x-errors
  url: https://cloud.google.com/resource-manager/docs/core_errors
- type: x-how-to-guides
  url: https://cloud.google.com/resource-manager/docs/how-to
- type: x-performance
  url: https://cloud.google.com/resource-manager/docs/performance
- type: x-pricing
  url: https://cloud.google.com/resource-manager/pricing
- type: x-rate-limits
  url: https://cloud.google.com/resource-manager/docs/limits
- type: x-website
  url: https://cloud.google.com/resource-manager/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---