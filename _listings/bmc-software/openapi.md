swagger: "2.0"
x-collection-name: BMC Software
x-complete: 1
info:
  title: BMC Software Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/events:
    post:
      summary: Create event
      description: Creates an event. Every event occurrence is persisted to the database
        as a RawEvent. Based on the EventFingerprint, a new Event will be created
        or an existing one will be de-duplicated.
      operationId: create-event
      x-api-path-slug: v1events-post
      responses:
        200:
          description: OK
      tags:
      - Events
    get:
      summary: List events
      description: Searches for events in the specified organization.
      operationId: list-events
      x-api-path-slug: v1events-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/raw:
    get:
      summary: List raw events
      description: Queries all event occurrences (raw events) for the specified organization.
      operationId: list-raw-events
      x-api-path-slug: v1eventsraw-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/:event_id:
    get:
      summary: Get event
      description: Returns the event with the specified event id from the database.
      operationId: get-event
      x-api-path-slug: v1eventsevent-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /v1/events/:event_id/raw:
    get:
      summary: Get raw events
      description: Returns all of the event occurrences (raw events) for the specified
        event.
      operationId: get-raw-events
      x-api-path-slug: v1eventsevent-idraw-get
      responses:
        200:
          description: OK
      tags:
      - Events
  /api/v1/events:
    post:
      summary: Post an Event
      description: This end point allows you to post events to the stream. You can
        tag them, set priority and event aggregate them with other events.
      operationId: post-an-event
      x-api-path-slug: apiv1events-post
      responses:
        200:
          description: OK
      tags:
      - ""