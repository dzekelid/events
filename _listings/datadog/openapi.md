swagger: "2.0"
x-collection-name: Datadog
x-complete: 1
info:
  title: DataDog Merged API
  version: 1.0.0
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    post:
      summary: Add Events
      description: Post an Event
      operationId: postEvents
      x-api-path-slug: events-post
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Events
  /events/:event_id:
    get:
      summary: Get Events Event
      description: GET events event
      operationId: getEventsEvent
      x-api-path-slug: eventsevent-id-get
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Events
      - Event
    delete:
      summary: Delete Events Event
      description: DELETE events event
      operationId: deleteEventsEvent
      x-api-path-slug: eventsevent-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Events
      - Event