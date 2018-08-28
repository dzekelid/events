---
swagger: "2.0"
x-collection-name: Actility
x-complete: 0
info:
  title: ThingPark DX Dataflow API Dataflow events retrieval
  description: Retrieves the list of events for all configured dataflows in scope.
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /dataflow/v021/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    get:
      summary: Dataflow events retrieval
      description: Retrieves the list of events for all configured dataflows in scope.
      operationId: retrieves-the-list-of-events-for-all-configured-dataflows-in-scope
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: dataflowRef
        description: Ref of the dataflow for which events should be retrieved
      responses:
        200:
          description: OK
      tags:
      - Dataflow
      - Events
      - Retrieval
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