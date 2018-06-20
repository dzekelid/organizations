---
swagger: "2.0"
x-collection-name: Open FinTech
x-complete: 1
info:
  title: Open FinTech
  description: openfintech-io-is-an-open-database-that-comprises-of-standardized-primary-data-for-fintech-industry--it-contains-such-information-as-geolocation-data-countries-cities-regions-organizations-currencies-national-digital-virtual-crypto-banks-digital-exchangers-payment-providers-psp-payment-methods-etc-it-is-created-for-communication-of-crossintegrated-microservices-on-one-language--this-is-achieved-through-standardization-of-entity-identifiers-that-are-used-to-exchange-information-among-different-services-
  version: "2017-08-24"
host: api.openfintech.io
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
      summary: List of organizations
      description: This endpoint retrievs the list of organizations present in the
        system. The data displays general, public information, without reference to
        the type of activity (for example - name, address, contacts, etc.).
      operationId: organizations.get
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: filter[industries]
        description: Filtering by industries
      - in: query
        name: filter[search]
        description: Full text search with id, name, code
      - in: query
        name: No Name
      - in: query
        name: sort
        description: Sort params:| ASC | DESC ||-----|------|| name | -name || code
          | -code || status | -status || description | -description |
      responses:
        200:
          description: OK
      tags:
      - Organizations
  /organizations/{id}:
    get:
      summary: Organization by ID
      description: Returns organization with specific ID.
      operationId: organizations.id.get
      x-api-path-slug: organizationsid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizations
---