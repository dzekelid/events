swagger: "2.0"
x-collection-name: AMEE
x-complete: 1
info:
  title: AMEE WRI Aqueduct API
  version: 1.0.0
host: api.roaring.io
basePath: /company/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /company-event:
    post:
      summary: Post Company Event
      description: Post company event.
      operationId: postCompanyEvent
      x-api-path-slug: companyevent-post
      parameters:
      - in: body
        name: body
        description: Request body with company identifiers to lookup
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Event