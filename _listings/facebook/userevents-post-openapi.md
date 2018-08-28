---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 0
info:
  title: Facebook Post User Events
  description: Creates an event for the user
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