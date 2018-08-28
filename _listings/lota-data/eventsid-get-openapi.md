---
swagger: "2.0"
x-collection-name: Lota Data
x-complete: 0
info:
  title: Lota Data Get Events
  description: Get specific event details..
  version: 2.0.0
host: api2.lotadata.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    get:
      summary: Get Events
      description: Find event occurrences in the area. returns results at specific
        place and time, event groups are expanded for every occurrence..
      operationId: events.get
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: activity
        description: List of required activity type ids (compliment to category)
      - in: query
        name: ambience
        description: List of required ambience ids
      - in: query
        name: bbox
        description: Corner of a bounding box (lat,lng)
      - in: query
        name: capacity_max
        description: Min capacity at location
      - in: query
        name: capacity_min
        description: Min capacity at location
      - in: query
        name: category
        description: List of required EventCategory ids (Tier 1)
      - in: query
        name: center
        description: latitude,longitude of the origin point
      - in: query
        name: fieldset
        description: Return results starting at specified offset (summary, context,
          detail)
      - in: query
        name: from_day
        description: Start on or after date specified (2015-10-16)
      - in: query
        name: genre
        description: List of required genre ids
      - in: query
        name: limit
        description: Max results to return
      - in: query
        name: name
        description: Matching on event and place names
      - in: query
        name: offset
        description: Return results starting at specified offset
      - in: query
        name: polygon
        description: Closed custom polygon
      - in: query
        name: q
        description: Text query matching titles, description, various text, tags,
          category
      - in: query
        name: radius
        description: Distance from origin in meters
      - in: query
        name: to_day
        description: Start on or before date specified (2015-10-16)
      - in: query
        name: within
        description: Search within specified geopolitical place id
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}:
    get:
      summary: Get Events
      description: Get specific event details..
      operationId: events.id.get
      x-api-path-slug: eventsid-get
      parameters:
      - in: query
        name: fieldset
      - in: path
        name: id
        description: event @id
      responses:
        200:
          description: OK
      tags:
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