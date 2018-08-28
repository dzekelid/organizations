---
name: NxtPort
x-slug: nxtport
description: NxtPort opens the gates to the Port of the future. This project is a
  milestone in the digitalization of logistics and cargo.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
x-kinRank: "7"
x-alexaRank: "3933231"
tags: Organizations
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apis.md
specificationVersion: "0.14"
apis:
- name: T-mining Secure Container Release API (live) - Register organization
  x-api-slug: apiv1organizations-post
  description: Register an Organization with a name. The name must be unique, so if
    one registers an Organization with a name that is already in use, an error will
    occur.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1organizations-post-openapi.md
- name: T-mining Secure Container Release API (live) - Create an Event
  x-api-slug: apiv1events-post
  description: |-
    Used to create an event for a container at a specific location and time.
    Each event is defined by a type.
    Currently a limited number of events (pickup and availability) are supported, but this may be extended with e.g. passage events.
    There are 2 ways to refer to a Container: by means of its id as defined in the Blockchain (this requires recording these ids in your app), or by means of a combination of the blNumber and isoNumber. Similarly, locations can be specified in 2 ways: by means of their id as defined in the Blockchain or by means of their name. In the latter case the name must be defined in a mapping   file for the Organization you - as a user- belong to. Also note that the container may not yet be known in the Blockchain at the time
    an availability event is created!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1events-post-openapi.md
- name: T-mining Secure Container Release API (live) - Register organization
  x-api-slug: apiv1organizations-post
  description: Register an Organization with a name. The name must be unique, so if
    one registers an Organization with a name that is already in use, an error will
    occur.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1organizations-post-openapi.md
- name: T-mining Secure Container Release API (live) - List PickupRights
  x-api-slug: apiv1pickup-rights-get
  description: Get all PickupRights that are assigned / transferred to the users's
    Organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1pickup-rights-get-openapi.md
- name: T-mining Secure Container Release API (live) - Revoke Transfer
  x-api-slug: apiv1pickup-rightsidrevoke-transfer-put
  description: Revoke the current PickupRight transfer. This must be used in case
    you did a transfer of a PickupRight to another Organization and you want to cancel
    this. This action is only possible as long as the PickupRight is not assigned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1pickup-rightsidrevoke-transfer-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1pickup-rightsidrevoke-transfer-put-openapi.md
- name: T-mining Secure Container Release API (live) - Transfer
  x-api-slug: apiv1pickup-rightsidtransfer-put
  description: Transfer the PickupRight to another Organization (a subcontractor).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1pickup-rightsidtransfer-put-openapi.md
- name: T-mining Secure Container Release API (live) - Block
  x-api-slug: apiv1releasesid-delete
  description: |-
    Blocking a release is done by a delete. This will revoke the PickupRight from the consignee. The Container and its PickupRight are deleted. Afterwards it is still possible to release again.
     The following conditions apply for this to work:
    * the container must have been released, i.e. there must be a vallid PickupRight   for the Container
    * the PickupRight should not be transferred to another Organization than the one that got the relesase initially
    * the PickupRight should not yet be assigned (to a driver / skipper)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1releasesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1releasesid-delete-openapi.md
- name: T-mining Secure Container Release API (live) - Register organization
  x-api-slug: apiv1organizations-post
  description: Register an Organization with a name. The name must be unique, so if
    one registers an Organization with a name that is already in use, an error will
    occur.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1organizations-post-openapi.md
- name: T-mining Secure Container Release API (live) - Create an Event
  x-api-slug: apiv1events-post
  description: |-
    Used to create an event for a container at a specific location and time.
    Each event is defined by a type.
    Currently a limited number of events (pickup and availability) are supported, but this may be extended with e.g. passage events.
    There are 2 ways to refer to a Container: by means of its id as defined in the Blockchain (this requires recording these ids in your app), or by means of a combination of the blNumber and isoNumber. Similarly, locations can be specified in 2 ways: by means of their id as defined in the Blockchain or by means of their name. In the latter case the name must be defined in a mapping   file for the Organization you - as a user- belong to. Also note that the container may not yet be known in the Blockchain at the time
    an availability event is created!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1events-post-openapi.md
- name: T-mining Secure Container Release API (live) - List PickupRights
  x-api-slug: apiv1pickup-rights-get
  description: Get all PickupRights that are assigned / transferred to the users's
    Organization.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1pickup-rights-get-openapi.md
- name: T-mining Secure Container Release API (live) - Revoke Transfer
  x-api-slug: apiv1pickup-rightsidrevoke-transfer-put
  description: Revoke the current PickupRight transfer. This must be used in case
    you did a transfer of a PickupRight to another Organization and you want to cancel
    this. This action is only possible as long as the PickupRight is not assigned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1pickup-rightsidrevoke-transfer-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1pickup-rightsidrevoke-transfer-put-openapi.md
- name: T-mining Secure Container Release API (live) - Transfer
  x-api-slug: apiv1pickup-rightsidtransfer-put
  description: Transfer the PickupRight to another Organization (a subcontractor).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1pickup-rightsidtransfer-put-openapi.md
- name: T-mining Secure Container Release API (live) - Block
  x-api-slug: apiv1releasesid-delete
  description: |-
    Blocking a release is done by a delete. This will revoke the PickupRight from the consignee. The Container and its PickupRight are deleted. Afterwards it is still possible to release again.
     The following conditions apply for this to work:
    * the container must have been released, i.e. there must be a vallid PickupRight   for the Container
    * the PickupRight should not be transferred to another Organization than the one that got the relesase initially
    * the PickupRight should not yet be assigned (to a driver / skipper)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1releasesid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1releasesid-delete-openapi.md
- name: T-mining Secure Container Release API (live) - Register organization
  x-api-slug: apiv1organizations-post
  description: Register an Organization with a name. The name must be unique, so if
    one registers an Organization with a name that is already in use, an error will
    occur.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1organizations-post-openapi.md
- name: T-mining Secure Container Release API (live) - Register organization
  x-api-slug: apiv1organizations-post
  description: Register an Organization with a name. The name must be unique, so if
    one registers an Organization with a name that is already in use, an error will
    occur.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28835-www-nxtport-eu.jpg
  humanURL: https://www.nxtport.eu
  baseURL: https://api.nxtport.eu//blockchain
  tags: Technology, SaaS, Enterprise, Shipping, Data, General Data, Relative Data,
    Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/organizations/master/_listings/nxtport/apiv1organizations-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://npr.api.gallery.streamdata.io
- type: x-api-stack
  url: http://nxtport.stack.network
- type: x-email
  url: mail@nxtport.eu
- type: x-email
  url: development@nxtport.eu
- type: x-email
  url: privacy@nxtport.eu
- type: x-github
  url: https://github.com/NxtPort
- type: x-openapi
  url: https://github.com/NxtPort/nxtport.github.io/tree/master/api
- type: x-twitter
  url: https://twitter.com/NxtPortNews
- type: x-website
  url: https://www.nxtport.eu
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---