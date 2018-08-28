---
swagger: "2.0"
x-collection-name: Netatmo
x-complete: 0
info:
  title: Netatmo Get Getnextevents
  description: Returns previous events.
  termsOfService: https://dev.netatmo.com/dev/resources/legal/introduction
  contact:
    name: Netatmo
    email: contact-api@netatmo.com
  version: 1.1.1
host: api.netatmo.net
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /geteventsuntil:
    get:
      summary: Get Geteventsuntil
      description: Returns the snapshot associated to an event.
      operationId: geteventsuntil
      x-api-path-slug: geteventsuntil-get
      parameters:
      - in: query
        name: event_id
        description: Your request will retrieve all the events until this one
      - in: query
        name: home_id
        description: ID of the Home youre interested in
      responses:
        200:
          description: OK
      tags:
      - Events
  /getnextevents:
    get:
      summary: Get Getnextevents
      description: Returns previous events.
      operationId: getnextevents
      x-api-path-slug: getnextevents-get
      parameters:
      - in: query
        name: event_id
        description: Your request will retrieve events occured before this one
      - in: query
        name: home_id
        description: ID of the Home youre interested in
      - in: query
        name: size
        description: Number of events to retrieve
      responses:
        200:
          description: OK
      tags:
      - Devices
      - Events
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