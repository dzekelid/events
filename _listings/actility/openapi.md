swagger: "2.0"
x-collection-name: Actility
x-complete: 1
info:
  title: ThingPark DX Maker API
  description: api-providing-features-for-device-makers-such-as-preprovisioning-on-standalone-join-servers-
  version: 1.0.0
host: dx-api.thingpark.com
basePath: /maker/v011/api
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