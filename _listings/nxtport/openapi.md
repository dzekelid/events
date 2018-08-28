swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/containers/{id}/events:
    get:
      summary: Get container events
      description: Get the list of Events related to a container
      operationId: getApiV1ContainersEvents
      x-api-path-slug: apiv1containersidevents-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: path
        name: id
        description: id of the Container
      responses:
        200:
          description: OK
      tags:
      - Container
      - Events