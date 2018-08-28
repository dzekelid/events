---
swagger: "2.0"
x-collection-name: Microsoft Office 365
x-complete: 0
info:
  title: Microsoft Office 365 Patch Events Event
  description: To update an event, send a PATCH request to the URL of the e...
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
  /Events{event_id}:
    get:
      summary: Get Events Event
      description: You can also retrieve information about a specific event by ...
      operationId: getEventsEvent
      x-api-path-slug: eventsevent-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
    delete:
      summary: Delete Events Event
      description: Upon success, the appointment is moved to the user's Deleted...
      operationId: deleteEventsEvent
      x-api-path-slug: eventsevent-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
    patch:
      summary: Patch Events Event
      description: To update an event, send a PATCH request to the URL of the e...
      operationId: patchEventsEvent
      x-api-path-slug: eventsevent-id-patch
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
      - Events
      - Event
    parameters:
      summary: Parameters Events Event
      description: Parameters events event
      operationId: parametersEventsEvent
      x-api-path-slug: eventsevent-id-parameters
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
  /Events{event_id}/Accept:
    post:
      summary: Add Events Event Accept
      description: Post events event  accept
      operationId: postEventsEventAccept
      x-api-path-slug: eventsevent-idaccept-post
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
      - Events
      - Event
      - ""
      - Accept
    parameters:
      summary: Parameters Events Event Accept
      description: Parameters events event  accept
      operationId: parametersEventsEventAccept
      x-api-path-slug: eventsevent-idaccept-parameters
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Accept
  /Events{event_id}/Decline:
    post:
      summary: Add Events Event Decline
      description: Post events event  decline
      operationId: postEventsEventDecline
      x-api-path-slug: eventsevent-iddecline-post
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
      - Events
      - Event
      - ""
      - Decline
    parameters:
      summary: Parameters Events Event Decline
      description: Parameters events event  decline
      operationId: parametersEventsEventDecline
      x-api-path-slug: eventsevent-iddecline-parameters
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Decline
  /Events{event_id}/TentativelyAccept:
    post:
      summary: Add Events Event Tentatively Accept
      description: Post events event  tentativelyaccept
      operationId: postEventsEventTentativelyaccept
      x-api-path-slug: eventsevent-idtentativelyaccept-post
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
      - Events
      - Event
      - ""
      - Tentativelyaccept
    parameters:
      summary: Parameters Events Event Tentatively Accept
      description: Parameters events event  tentativelyaccept
      operationId: parametersEventsEventTentativelyaccept
      x-api-path-slug: eventsevent-idtentativelyaccept-parameters
      responses:
        200:
          description: OK
      tags:
      - Events
      - Event
      - ""
      - Tentativelyaccept
  /Messages{event_id}/Send:
    post:
      summary: Add Messages Event Send
      description: You can send an existing email that has the IsDraft property...
      operationId: postMessagesEventSend
      x-api-path-slug: messagesevent-idsend-post
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Event
      - ""
      - Send
    parameters:
      summary: Parameters Messages Event Send
      description: Parameters messages event  send
      operationId: parametersMessagesEventSend
      x-api-path-slug: messagesevent-idsend-parameters
      responses:
        200:
          description: OK
      tags:
      - Messages
      - Event
      - ""
      - Send
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