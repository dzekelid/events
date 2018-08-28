swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 1
info:
  title: OpenDNS
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    put:
      summary: Post Event
      description: Posts a Malware event to the API for processing and optionally
        adding to a customer's domain lists.
      operationId: postEvent
      x-api-path-slug: events-put
      responses:
        200:
          description: OK
      tags:
      - Event