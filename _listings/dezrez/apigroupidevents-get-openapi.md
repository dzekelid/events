---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get group events by its Id
  version: 1.0.0
  description: Get group events by its id.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/group/{id}/events:
    get:
      summary: Get group events by its Id
      description: Get group events by its id.
      operationId: Group_EventsByidBypageSizeBypageNumberBybranchIdByfromBytoBytypeByeventCategoryTypeByactiveRolesOnly
      x-api-path-slug: apigroupidevents-get
      parameters:
      - in: query
        name: activeRolesOnly
        description: Only return active roles
      - in: query
        name: branchId
      - in: query
        name: eventCategoryType
        description: An event category type to return
      - in: query
        name: excludedTypes
        description: Bring back all except these types
      - in: query
        name: from
        description: the date from
      - in: path
        name: id
        description: The id of the group to get events for
      - in: query
        name: includeDrafts
      - in: query
        name: pageNumber
        description: The page of events to return
      - in: query
        name: pageSize
        description: The number of events to return
      - in: query
        name: propertyId
        description: The property the event must relate to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      - in: query
        name: to
        description: the date to
      - in: query
        name: type
        description: The event type to get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Events
      - By
      - Its
      - Id
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