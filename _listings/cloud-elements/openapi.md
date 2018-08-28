swagger: "2.0"
x-collection-name: Cloud Elements
x-complete: 1
info:
  title: zohocrm
  version: api-v2
host: console.cloud-elements.com
basePath: /elements/api-v2/hubs/crm
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /log/get_events:
    post:
      summary: Get Events
      description: Get events.
      operationId: postLogGetEvents
      x-api-path-slug: logget-events-post
      parameters:
      - in: query
        name: category
        description: optional filter the returned events to a single category (see
          Event types below)
      - in: query
        name: cursor
        description: optional encoded value indicating from what point to get the
          next limit logs
      - in: query
        name: end_ts
        description: optional end time (UTC timestamp in milliseconds since the Unix
          epoch)
      - in: query
        name: limit
        description: optional number of results to return per call (default 1000,
          maximum 1000)
      - in: query
        name: start_ts
        description: optional start time (UTC timestamp in milliseconds since the
          Unix epoch)
      - in: query
        name: user
        description: optional member ID, user ID, or email of a user for filtering
          events
      responses:
        200:
          description: OK
      tags:
      - Events