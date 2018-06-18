---
swagger: "2.0"
x-collection-name: Data2CRM
x-complete: 0
info:
  title: Data2CRM GET for Event
  description: Return event information
  version: "1"
host: api.data2crm.com:80
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /event:
    get:
      summary: GET for Event
      description: Returns all events from the system
      operationId: getEventCollection
      x-api-path-slug: event-get
      parameters:
      - in: query
        name: filter
        description: Filter
      - in: query
        name: limit
        description: 'Amount of results (default: 25)'
      - in: query
        name: offset
        description: 'Start from record (default: 0)'
      - in: query
        name: parent_id
        description: Parent Identifier
      - in: query
        name: parent_type
        description: Parent Type
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-DATA-ENABLE
        description: Data Enable
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
    post:
      summary: POST for Event
      description: Add event into the system
      operationId: createEventEntity
      x-api-path-slug: event-post
      parameters:
      - in: body
        name: body
        description: Add event into the system
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
  /event/count:
    get:
      summary: COUNT for Event
      description: Count all events from the system
      operationId: getEventCountCollection
      x-api-path-slug: eventcount-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
      - Count
  /event/describe:
    get:
      summary: DESCRIBE for Event
      description: Returns describe for events
      operationId: getEventDescribe
      x-api-path-slug: eventdescribe-get
      parameters:
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
      - Describe
  /event/{event_id}:
    delete:
      summary: DELETE for Event
      description: Delete event information
      operationId: deleteEventEntity
      x-api-path-slug: eventevent-id-delete
      parameters:
      - in: path
        name: event_id
        description: Event Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
      - Events
    get:
      summary: GET for Event
      description: Return event information
      operationId: getEventEntity
      x-api-path-slug: eventevent-id-get
      parameters:
      - in: path
        name: event_id
        description: Event Identifier
      - in: header
        name: X-API2CRM-CRMKEY
        description: CRM Key
      - in: header
        name: X-API2CRM-USERKEY
        description: User Key
      responses:
        200:
          description: OK
      tags:
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