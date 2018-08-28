---
swagger: "2.0"
x-collection-name: Datadog
x-complete: 0
info:
  title: DataDog API Delete Events Event
  version: 1.0.0
  description: DELETE events event
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