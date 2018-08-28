swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
basePath: /1
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