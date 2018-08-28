---
swagger: "2.0"
x-collection-name: ATTOM
x-complete: 0
info:
  title: Attom Data Solutions API Returns all the events that have occurred on a specific
    address.
  description: Get a detail of all the events on a specific property based on its
    address.
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