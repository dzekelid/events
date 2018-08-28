swagger: "2.0"
x-collection-name: Twine
x-complete: 1
info:
  title: Twine
  description: -overviewthe-twine-health-api-is-restful-api--the-requests-and-responses-are-formated-according-to-the-json-apihttpjsonapi-orgformat1-0-specification-in-addition-to-this-documentation-we-also-provide-an-openapihttpsgithub-comoaiopenapispecificationblobmasterversions2-0-md-yaml-file-describing-the-api-twine-api-specificationswagger-yaml--authenticationauthentication-for-the-twine-api-is-based-on-the-oauth-2-0-authorization-frameworkhttpstools-ietf-orghtmlrfc6749--twine-currently-supports-grant-types-of-client-credentials-and-refresh-token-see-post-oauthtokenoperationcreatetoken-for-details-on-the-request-and-response-formats--redocinject-securitydefinitions-
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calendar_event:
    get:
      summary: List calendar events
      description: Get a list of calendar events
      operationId: fetchCalendarEvents
      x-api-path-slug: calendar-event-get
      parameters:
      - in: query
        name: filter[attendees]
        description: Comma-separated list of coach or patient ids
      - in: query
        name: filter[completed]
        description: If not specified, return all calendar events
      - in: query
        name: filter[completed_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[created_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[end_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[groups]
        description: Comma-separated list of group ids
      - in: query
        name: filter[organization]
        description: Twine organization id
      - in: query
        name: filter[patient]
        description: Patient id to fetch calendar event
      - in: query
        name: filter[start_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: filter[type]
        description: Calendar event type
      - in: query
        name: filter[updated_at]
        description: The start (inclusive) and end (exclusive) dates are ISO date
          and time strings separated by `
      - in: query
        name: include
        description: List of related resources to include in the response
      - in: query
        name: page[number]
        description: Page number
      - in: query
        name: page[size]
        description: Page size
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - List
      - Calendar
      - Events
    post:
      summary: Create calendar event
      description: Create a calendar event for a patient. Attribute `all_day` must
        be set to `true` and `end_at` cannot be set for `plan-check-in` event type.
      operationId: createCalendarEvent
      x-api-path-slug: calendar-event-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Calendar
      - Event
  /calendar_event/{id}:
    delete:
      summary: Delete a calendar event
      description: Delete a calendar event by id
      operationId: deleteCalendarEvent
      x-api-path-slug: calendar-eventid-delete
      parameters:
      - in: path
        name: id
        description: Calendar event identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Calendar
      - Event
    get:
      summary: Get a calendar event
      description: Get a calendar event by id
      operationId: fetchCalendarEvent
      x-api-path-slug: calendar-eventid-get
      parameters:
      - in: path
        name: id
        description: Calendar event identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Calendar
      - Event
    patch:
      summary: Update a calendar event
      description: Update a calendar event for a patient. Attribute `all_day` must
        be true and `end_at` cannot be specified for `plan-check-in` event type. To
        mark a calendar event as 'completed', set `completed_at` and `completed_by`
        to desired values.  To mark a completed calendar event as 'not completed',
        set `completed_at` and `completed_by` to `null`.
      operationId: updateCalendarEvent
      x-api-path-slug: calendar-eventid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Calendar event identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Calendar
      - Event