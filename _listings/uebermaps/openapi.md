swagger: "2.0"
x-collection-name: uebermaps
x-complete: 1
info:
  title: uebermaps
  description: enable-people-to-store-spots-on-public-and-private-maps
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
  /spots/{id}/events:
    get:
      summary: List events for a given spot
      description: List maps for a given spot.
      operationId: spots.id.events.get
      x-api-path-slug: spotsidevents-get
      parameters:
      - in: query
        name: bounds
        description: To refine your event index request to contain only events within                                                             a
          geographical box pass the followng bounds parameters
      - in: path
        name: id
        description: Id of spot
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
      - Eventsa
      - Given
      - Spot
    post:
      summary: Create event
      description: Create event. Wrap map parameters in [event].
      operationId: spots.id.events.post
      x-api-path-slug: spotsidevents-post
      parameters:
      - in: body
        name: event
        description: Event attributes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Spot id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Event
  /events/{id}:
    delete:
      summary: Delete event
      description: Delete event.
      operationId: events.id.delete
      x-api-path-slug: eventsid-delete
      parameters:
      - in: path
        name: id
        description: Event id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Event
    get:
      summary: Get event
      description: Get basic information about an event
      operationId: events.id.get
      x-api-path-slug: eventsid-get
      parameters:
      - in: path
        name: id
        description: Id of event
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Event
    patch:
      summary: Update event
      description: Update event. Wrap event parameters in [event].
      operationId: events.id.patch
      x-api-path-slug: eventsid-patch
      parameters:
      - in: body
        name: event
        description: Event attributes
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Event id
      responses:
        200:
          description: OK
      tags:
      - Mapping
      - Event