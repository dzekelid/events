swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /allevents/detail:
    get:
      summary: Returns all the events that have occurred on a specific address.
      description: Get a detail of all the events on a specific property based on
        its address.
      operationId: getAllEventsDetailAddress
      x-api-path-slug: alleventsdetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: API Security Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - ""
      - Events
      - That
      - Have
      - Occurred
      - "On"
      - Specific
      - Address