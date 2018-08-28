---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph Create Event
  description: Create Event Use this API to create a new Event in the default or the
    specified calendar.
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new Event in the default
        or the specified calendar.
      operationId: CreateEvent
      x-api-path-slug: mecalendarevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new Event in the default
        or the specified calendar.
      operationId: CreateEvent
      x-api-path-slug: usersid--userprincipalnamecalendarevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new event.
      operationId: CreateEvent
      x-api-path-slug: groupsidcalendarevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new Event in the default
        or the specified calendar.
      operationId: CreateEvent
      x-api-path-slug: mecalendarsidevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new Event in the default
        or the specified calendar.
      operationId: CreateEvent
      x-api-path-slug: usersid--userprincipalnamecalendarsidevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new Event in the default
        or the specified calendar.
      operationId: CreateEvent
      x-api-path-slug: mecalendargroupcalendarsidevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new Event in the default
        or the specified calendar.
      operationId: CreateEvent
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsidevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new Event in the default
        or the specified calendar.
      operationId: CreateEvent
      x-api-path-slug: mecalendargroupsidcalendarsidevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new Event in the default
        or the specified calendar.
      operationId: CreateEvent
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsidevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Use this API to create a new event.
      operationId: CreateEvent
      x-api-path-slug: groupsidevents-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
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
    post:
      summary: Create Event
      description: Create Event Create an event in the user's default calendar.
      operationId: CreateEvent
      x-api-path-slug: usersid--userprincipalnameevents-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /me/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: meeventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /users/{id | userPrincipalName}/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: usersid--userprincipalnameeventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /groups/{id}/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: groupsideventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /me/calendar/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: mecalendareventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /users/{id | userPrincipalName}/calendar/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: usersid--userprincipalnamecalendareventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /groups/{id}/calendar/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: groupsidcalendareventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /me/calendars/{id}/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: mecalendarsideventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /me/calendargroup/calendars/{id}/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: mecalendargroupcalendarsideventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /me/calendargroups/{id}/calendars/{id}/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: mecalendargroupsidcalendarsideventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/accept:
    post:
      summary: Event Accept
      description: 'event: accept Accept the specified event.'
      operationId: Event:Accept
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsidaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Accept
  /me/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: meeventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /users/{id | userPrincipalName}/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: usersid--userprincipalnameeventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /groups/{id}/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: groupsideventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /me/calendar/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: mecalendareventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /users/{id | userPrincipalName}/calendar/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: usersid--userprincipalnamecalendareventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /groups/{id}/calendar/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: groupsidcalendareventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /me/calendars/{id}/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: mecalendarsideventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /me/calendargroup/calendars/{id}/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: mecalendargroupcalendarsideventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /me/calendargroups/{id}/calendars/{id}/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: mecalendargroupsidcalendarsideventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/decline:
    post:
      summary: Event Decline
      description: 'event: decline Decline invitation to the specified event.'
      operationId: Event:Decline
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsiddecline-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Decline
  /me/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: meeventsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: meeventsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: meeventsid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /users/{id | userPrincipalName}/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: usersid--userprincipalnameeventsid-delete
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
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: usersid--userprincipalnameeventsid-get
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
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: usersid--userprincipalnameeventsid-patch
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
      responses:
        200:
          description: OK
      tags:
      - Event
  /groups/{id}/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: groupsideventsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: groupsideventsid-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: groupsideventsid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer %token%
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /me/calendar/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: mecalendareventsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: mecalendareventsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: mecalendareventsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /users/{id | userPrincipalName}/calendar/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: usersid--userprincipalnamecalendareventsid-delete
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
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: usersid--userprincipalnamecalendareventsid-get
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
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: usersid--userprincipalnamecalendareventsid-patch
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
      responses:
        200:
          description: OK
      tags:
      - Event
  /groups/{id}/calendar/events/{id}/:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: groupsidcalendareventsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /me/calendars/{id}/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: mecalendarsideventsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: mecalendarsideventsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: mecalendarsideventsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsid-delete
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
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsid-get
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
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsid-patch
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
      responses:
        200:
          description: OK
      tags:
      - Event
  /me/calendargroup/calendars/{id}/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: mecalendargroupcalendarsideventsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: mecalendargroupcalendarsideventsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: mecalendargroupcalendarsideventsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsid-delete
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
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsid-get
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
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsid-patch
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
      responses:
        200:
          description: OK
      tags:
      - Event
  /me/calendargroups/{id}/calendars/{id}/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: mecalendargroupsidcalendarsideventsid-delete
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: mecalendargroupsidcalendarsideventsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: mecalendargroupsidcalendarsideventsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}:
    delete:
      summary: Delete Event
      description: Delete event Delete event.
      operationId: DeleteEvent
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsid-delete
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
      responses:
        200:
          description: OK
      tags:
      - Event
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsid-get
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
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsid-patch
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
      responses:
        200:
          description: OK
      tags:
      - Event
  /me/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: meeventsiddismissreminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /users/{id | userPrincipalName}/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: usersid--userprincipalnameeventsiddismissreminder-post
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
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /groups/{id}/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: groupsideventsiddismissreminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /me/calendar/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: mecalendareventsiddismissreminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /users/{id | userPrincipalName}/calendar/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: usersid--userprincipalnamecalendareventsiddismissreminder-post
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
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /groups/{id}/calendar/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: groupsidcalendareventsiddismissreminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /me/calendars/{id}/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: mecalendarsideventsiddismissreminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsiddismissreminder-post
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
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /me/calendargroup/calendars/{id}/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: mecalendargroupcalendarsideventsiddismissreminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsiddismissreminder-post
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
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /me/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: mecalendargroupsidcalendarsideventsiddismissreminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/dismissReminder:
    post:
      summary: Event Dismiss Reminder
      description: 'event: dismissReminder Dissmiss a reminder that has been triggered.'
      operationId: Event:DismissReminder
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsiddismissreminder-post
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
      responses:
        200:
          description: OK
      tags:
      - Event
      - Dismiss
      - Reminder
  /groups/{id}/calendar/events/{id}:
    get:
      summary: Get Event
      description: Get event Get the properties and relationships of the specified
        event object.
      operationId: GetEvent
      x-api-path-slug: groupsidcalendareventsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
    patch:
      summary: Update Event
      description: Update event Update the properties of event object.
      operationId: UpdateEvent
      x-api-path-slug: groupsidcalendareventsid-patch
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
  /me/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: meeventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /users/{id | userPrincipalName}/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: usersid--userprincipalnameeventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /groups/{id}/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: groupsideventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /me/calendar/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: mecalendareventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /users/{id | userPrincipalName}/calendar/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: usersid--userprincipalnamecalendareventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /groups/{id}/calendar/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: groupsidcalendareventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /me/calendars/{id}/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: mecalendarsideventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /me/calendargroup/calendars/{id}/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: mecalendargroupcalendarsideventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /me/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: mecalendargroupsidcalendarsideventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/snoozeReminder:
    post:
      summary: Event Snooze Reminder
      description: 'event: snoozeReminder Postpone a reminder until a new time.'
      operationId: Event:SnoozeReminder
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsidsnoozereminder-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Snooze
      - Reminder
  /me/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: meeventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /users/{id | userPrincipalName}/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: usersid--userprincipalnameeventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /groups/{id}/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: groupsideventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /me/calendar/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: mecalendareventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /users/{id | userPrincipalName}/calendar/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: usersid--userprincipalnamecalendareventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /groups/{id}/calendar/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: groupsidcalendareventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /me/calendars/{id}/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: mecalendarsideventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /me/calendargroup/calendars/{id}/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: mecalendargroupcalendarsideventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /me/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: mecalendargroupsidcalendarsideventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/tentativelyAccept:
    post:
      summary: Event Tentatively Accept
      description: 'event: tentativelyAccept Tentatively accept the specified event.'
      operationId: Event:TentativelyAccept
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsidtentativelyaccept-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: Nature of the data in the body of an entity
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - Event
      - Tentatively
      - Accept
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