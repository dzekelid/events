---
swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 0
info:
  title: OpenDNS Post Event
  version: 1.0.0
  description: Posts a Malware event to the API for processing and optionally adding
    to a customer's domain lists.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    put:
      summary: Post Event
      description: Posts a Malware event to the API for processing and optionally
        adding to a customer's domain lists.
      operationId: postEvent
      x-api-path-slug: events-put
      responses:
        200:
          description: OK
      tags:
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