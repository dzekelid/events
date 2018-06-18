---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/calendar/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: mecalendarevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/calendar/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnamecalendarevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /groups/{id}/calendar/events:
    get:
      summary: List Events
      description: List events Retrieve a list of event objects.
      operationId: ListEvents
      x-api-path-slug: groupsidcalendarevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /me/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: mecalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnamecalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /me/calendarGroup/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: mecalendargroupcalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /me/calendarGroups/{id}/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: mecalendargroupsidcalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /groups/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of event objects.
      operationId: ListEvents
      x-api-path-slug: groupsidevents-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/events:
    get:
      summary: List Events
      description: List events Get a list of event objects in the user's mailbox.
        The list contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnameevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
---