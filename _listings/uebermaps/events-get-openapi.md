---
swagger: "2.0"
x-collection-name: uebermaps
x-complete: 0
info:
  title: uebermaps List your own events
  description: List your own events.
  termsOfService: https://uebermaps.com/terms/
  contact:
    name: uebermaps API Team
  version: "2.0"
host: uebermaps.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    get:
      summary: List your own events
      description: List your own events.
      operationId: events.get
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: bounds
        description: To refine your event index request to contain only events within                                                             a
          geographical box pass the followng bounds parameters
      - in: query
        name: timeframe_end
        description: End of time range of event (ISO 8601 date format)
      - in: query
        name: timeframe_start
        description: Begin of time range of event (ISO 8601 date format)
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Your
      - Own
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