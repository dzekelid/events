---
swagger: "2.0"
x-collection-name: PredictHQ
x-complete: 0
info:
  title: PredictHQ Retrieve Events Calendar
  description: |-
    This endpoint accepts the same parameters as the ones described in Retrieve All Events and can be used to get a calendar view of all matching events that are available to your account.

    Each day in the calendar contains aggregate counts of all _active_ events for that day.
  version: 1.0.0
host: api.predicthq.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/events/calendar/:
    get:
      summary: Retrieve Events Calendar
      description: |-
        This endpoint accepts the same parameters as the ones described in Retrieve All Events and can be used to get a calendar view of all matching events that are available to your account.

        Each day in the calendar contains aggregate counts of all _active_ events for that day.
      operationId: V1EventsCalendarGet
      x-api-path-slug: v1eventscalendar-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Calendar
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