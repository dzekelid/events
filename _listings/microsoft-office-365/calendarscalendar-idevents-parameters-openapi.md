---
swagger: "2.0"
x-collection-name: Microsoft Office 365
x-complete: 0
info:
  title: Microsoft Office 365 Parameters Calendars Calendar Events
  description: Parameters calendars calendar  events
  version: 1.0.0
host: outlook.office365.com
basePath: /ews/odata/Me
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Calendars{calendar_id}/Events:
    get:
      summary: Get Calendars Calendar Events
      description: You can request all the events across all calendars (or a fi...
      operationId: getCalendarsCalendarEvents
      x-api-path-slug: calendarscalendar-idevents-get
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
      - ""
      - Events
    post:
      summary: Add Calendars Calendar Events
      description: Post calendars calendar  events
      operationId: postCalendarsCalendarEvents
      x-api-path-slug: calendarscalendar-idevents-post
      parameters:
      - in: body
        name: body
        description: (Untitled)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
      - ""
      - Events
    parameters:
      summary: Parameters Calendars Calendar Events
      description: Parameters calendars calendar  events
      operationId: parametersCalendarsCalendarEvents
      x-api-path-slug: calendarscalendar-idevents-parameters
      responses:
        200:
          description: OK
      tags:
      - Calendars
      - Calendar
      - ""
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