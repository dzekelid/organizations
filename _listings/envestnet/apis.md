---
name: Envestnet
x-slug: envestnet
description: Build and transform financial apps and services with access to financial
  data through our APIs and digital solutions for banks, developers, and innovators.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
x-kinRank: "8"
x-alexaRank: "84912"
tags: Organizations
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/envestnet/apis.md
specificationVersion: "0.14"
apis:
- name: Crunch Base Organizations
  x-api-slug: crunch-base
  description: Get Organizations
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//organizations
  tags: Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/envestnet/organizations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/envestnet/organizations-get-openapi.md
- name: Crunch Base Get Organizations
  x-api-slug: crunch-base
  description: Get Organization Using Permalink
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//organizations/{permalink}
  tags: Organizations,Permalink
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/envestnet/organizationspermalink-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/envestnet/organizationspermalink-get-openapi.md
- name: Crunch Base Get Organization Relationships
  x-api-slug: crunch-base
  description: Get Organizations Relationships Using Permlink
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3//organizations/{permalink}/{relationship_name}
  tags: Organizations,Permalink,Relationship,Name
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/envestnet/organizationspermalinkrelationship-name-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/envestnet/organizationspermalinkrelationship-name-get-openapi.md
- name: Crunch Base
  x-api-slug: crunch-base
  description: Build and transform financial apps and services with access to financial
    data through our APIs and digital solutions for banks, developers, and innovators.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1691-yodlee.jpg
  humanURL: http://www.yodlee.com/
  baseURL: https://api.crunchbase.com//v/3
  tags: Organizations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/envestnet/openapi.md
x-common:
- type: x-base
  url: https://rest.developer.yodlee.com/services/srest/
- type: x-blog
  url: http://www.yodlee.com/yodlee-moneycenter-blog/
- type: x-blog-rss
  url: http://www.yodlee.com/yodlee-moneycenter-blog/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/yodlee
- type: x-crunchbase
  url: https://crunchbase.com/organization/yodlee
- type: x-developer
  url: http://developer.yodlee.com/
- type: x-email
  url: Customercare@yodlee.com
- type: x-email
  url: customerservice@yodlee.com
- type: x-github
  url: https://github.com/Yodlee
- type: x-twitter
  url: https://twitter.com/Yodlee
- type: x-website
  url: http://www.yodlee.com/
- type: x-website
  url: http://crunchbase.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---