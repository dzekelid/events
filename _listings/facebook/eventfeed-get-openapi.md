---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Get Event Feed
  description: This event's wall
  version: 1.0.0
host: graph.facebook.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{page}/events:
    get:
      summary: Get Page Events
      description: The events the Page is attending
      operationId: getPageEvents
      x-api-path-slug: pageevents-get
      parameters:
      - in: path
        name: page
        description: Represents the ID of the page object
      responses:
        200:
          description: OK
      tags:
      - Page
      - Events
    post:
      summary: Post Page Events
      description: Creates an event for the page
      operationId: postPageEvents
      x-api-path-slug: pageevents-post
      parameters:
      - in: query
        name: end_time
        description: Event end time
      - in: query
        name: location
        description: Event location
      - in: query
        name: message
        description: Event description
      - in: query
        name: name
        description: Event name
      - in: path
        name: page
        description: Represents the ID of the page object
      - in: query
        name: privacy_type
        description: Event privacy setting
      - in: query
        name: start_time
        description: Event start time
      responses:
        200:
          description: OK
      tags:
      - Page
      - Events
  /{user}/events:
    get:
      summary: Get User Events
      description: The events this user is attending.
      operationId: getUserEvents
      x-api-path-slug: userevents-get
      parameters:
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Events
    post:
      summary: Post User Events
      description: Creates an event for the user
      operationId: postUserEvents
      x-api-path-slug: userevents-post
      parameters:
      - in: query
        name: end_time
        description: Event end time
      - in: query
        name: location
        description: Event location
      - in: query
        name: message
        description: Event description
      - in: query
        name: name
        description: Event name
      - in: query
        name: privacy_type
        description: Event privacy setting
      - in: query
        name: start_time
        description: Event start time
      - in: path
        name: user
        description: Represents the ID of the user object
      responses:
        200:
          description: OK
      tags:
      - User
      - Events
  /{event}:
    get:
      summary: Get Event
      description: Specifies information about an event, including the location, event
        name, and which invitees plan to attend.
      operationId: getEvent
      x-api-path-slug: event-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
  /{event}/feed:
    get:
      summary: Get Event Feed
      description: This event's wall
      operationId: getEventFeed
      x-api-path-slug: eventfeed-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Feed
    post:
      summary: Post Event Feed
      description: Posts a status message on this event's wall
      operationId: postEventFeed
      x-api-path-slug: eventfeed-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      - in: query
        name: message
        description: Status Message content
      responses:
        200:
          description: OK
      tags:
      - Event
      - Feed
  /{event}/noreply:
    get:
      summary: Get Event Noreply
      description: All of the users who have been not yet responded to their invitation
        to this event
      operationId: getEventNoreply
      x-api-path-slug: eventnoreply-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Noreply
  /{event}/maybe:
    get:
      summary: Get Event Maybe
      description: All of the users who have been responded "Maybe" to their invitation
        to this event
      operationId: getEventMaybe
      x-api-path-slug: eventmaybe-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Maybe
    post:
      summary: Post Event Maybe
      description: RSVPs the user as a 'maybe' for the event
      operationId: postEventMaybe
      x-api-path-slug: eventmaybe-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Maybe
  /{event}/invited:
    get:
      summary: Get Event Invited
      description: All of the users who have been invited to this event
      operationId: getEventInvited
      x-api-path-slug: eventinvited-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Invited
  /{event}/attending:
    get:
      summary: Get Event Attending
      description: All of the users who are attending this event
      operationId: getEventAttending
      x-api-path-slug: eventattending-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Attending
    post:
      summary: Post Event Attending
      description: RSVPs the user as 'attending' for the event
      operationId: postEventAttending
      x-api-path-slug: eventattending-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Attending
  /{event}/declined:
    get:
      summary: Get Event Declined
      description: All of the users who declined their invitation to this event
      operationId: getEventDeclined
      x-api-path-slug: eventdeclined-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Declined
    post:
      summary: Post Event Declined
      description: RSVPs the user as 'declined' for the event
      operationId: postEventDeclined
      x-api-path-slug: eventdeclined-post
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      responses:
        200:
          description: OK
      tags:
      - Event
      - Declined
  /{event}/picture:
    get:
      summary: Get Event Picture
      description: The event's profile picture
      operationId: getEventPicture
      x-api-path-slug: eventpicture-get
      parameters:
      - in: path
        name: event
        description: Represents the ID of the event object
      - in: query
        name: type
        description: One of square (50x50), small (50 pixels wide, variable height),
          and large (about 200 pixels wide,                                                        variable
          height)
      responses:
        200:
          description: OK
      tags:
      - Event
      - Picture
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