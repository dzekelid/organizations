---
name: Open FinTech
x-slug: open-fintech
description: International standards yield technological, economic and social advantages.
  Standards speed up the development of new applications and simplify the process
  of communication between the services. Data and service is available under the Open
  Database License (ODbL). It is an open standard and open data, every player of FinTech
  market can contribute to development and enhancement. All data is available through
  Rest API based on JSON API standard.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/open-fintech-io.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Organizations
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/open-fintech/apis.md
specificationVersion: "0.14"
apis:
- name: Open FinTech List of organizations
  x-api-slug: open-fintech
  description: This endpoint retrievs the list of organizations present in the system.
    The data displays general, public information, without reference to the type of
    activity (for example - name, address, contacts, etc.).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/open-fintech-io.png
  humanURL: http://openfintech.io
  baseURL: https://api.openfintech.io//v1///organizations
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/open-fintech/organizations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/open-fintech/organizations-get-openapi.md
- name: Open FinTech Organization by ID
  x-api-slug: open-fintech
  description: Returns organization with specific ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/open-fintech-io.png
  humanURL: http://openfintech.io
  baseURL: https://api.openfintech.io//v1///organizations/{id}
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/open-fintech/organizationsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/open-fintech/organizationsid-get-openapi.md
- name: Open FinTech
  x-api-slug: open-fintech
  description: International standards yield technological, economic and social advantages.
    Standards speed up the development of new applications and simplify the process
    of communication between the services. Data and service is available under the
    Open Database License (ODbL). It is an open standard and open data, every player
    of FinTech market can contribute to development and enhancement. All data is available
    through Rest API based on JSON API standard.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/open-fintech-io.png
  humanURL: http://openfintech.io
  baseURL: https://api.openfintech.io//v1/
  tags: Organizations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/open-fintech/openapi.md
x-common:
- type: x-developer
  url: https://docs.openfintech.io/
- type: x-getting-started
  url: https://docs.openfintech.io/#section/Get-Started
- type: x-github
  url: https://github.com/openfintechio
- type: x-website
  url: http://openfintech.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---