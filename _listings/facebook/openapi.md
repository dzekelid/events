---
swagger: "2.0"
x-collection-name: Facebook
x-complete: 1
info:
  title: Facebook
  description: connect-to-the-social-network-with-the-graph-api-
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
---