---
name: Gitter
x-slug: gitter
description: Gitter is a chat and networking platform that helps to manage, grow and
  connect communities through messaging, content and discovery.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
x-kinRank: "8"
x-alexaRank: "18282"
tags: Organizations
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/gitter/apis.md
specificationVersion: "0.14"
apis:
- name: Gitter API User Orgs
  x-api-slug: gitter-api
  description: List of the user's GitHub Organisations and their respective Room if
    available.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https://///user/:userId/orgs
  tags: Users,Organizations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/gitter/useruseridorgs-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/gitter/useruseridorgs-get-openapi.md
- name: Gitter API
  x-api-slug: gitter-api
  description: Gitter is a chat and networking platform that helps to manage, grow
    and connect communities through messaging, content and discovery.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/gitter-logo.png
  humanURL: http://gitter.im
  baseURL: https:///
  tags: Organizations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/gitter/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/gitter
- type: x-developer
  url: https://developer.gitter.im/docs/streaming-api
- type: x-github
  url: https://github.com/gitterHQ
- type: x-curated-source
  url: https://gitter.im/apiaryio/api-blueprint
- type: x-website
  url: http://gitter.im
- type: x-twitter
  url: https://twitter.com/gitchat
- type: x-website
  url: https://gitter.im
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---