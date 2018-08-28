---
swagger: "2.0"
info:
  title: Meetup batch
  description: Performs multiple API requests in batch, useful for reducing HTTP network
    requests. This method is only available for OAuth authentication
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /batch:
    post:
      summary: batch
      description: Performs multiple API requests in batch, useful for reducing HTTP
        network requests
      operationId: batch
      parameters:
      - in: query
        name: requests
        description: JSON-encoding of multiple request objects as described in the
          parameter notes
        type: string
      responses:
        200:
          description: OK
      tags:
      - events
      - batch
definitions: []
x-collection-name: Meetup
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