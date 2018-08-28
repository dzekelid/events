---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve the change history of the set of rules for a custom event
  description: |-
    Retrieve the change history of the set of rules for the selected custom event.
    The history is updated each time you change the rules.
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /custom-events:
    get:
      summary: Retrieve a list of custom events
      description: Retrieve a list of custom events
      operationId: retrieve-a-list-of-custom-events
      x-api-path-slug: customevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Custom
      - Events
    post:
      summary: Create a custom event
      description: Create a custom event
      operationId: create-a-custom-event
      x-api-path-slug: customevents-post
      parameters:
      - in: body
        name: body
        description: Custom event resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Event
  /events:
    get:
      summary: Retrieve a list of existing events
      description: ""
      operationId: ""
      x-api-path-slug: events-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Existing
      - Events
  /queue/custom-events:
    get:
      summary: Retrieve a list of scheduled custom events
      description: Retrieve a list of scheduled custom events
      operationId: retrieve-a-list-of-scheduled-custom-events
      x-api-path-slug: queuecustomevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Scheduled
      - Custom
      - Events
  /custom-events/{id}:
    delete:
      summary: Delete a custom event
      description: Delete a custom event with predefined identifier string
      operationId: delete-a-custom-event-with-predefined-identifier-string
      x-api-path-slug: customeventsid-delete
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Event
    get:
      summary: Retrieve a custom event
      description: Retrieve a custom event with predefined identifier string
      operationId: retrieve-a-custom-event-with-predefined-identifier-string
      x-api-path-slug: customeventsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Custom
      - Event
    put:
      summary: Create a custom event with predefined ID
      description: Create a custom event with predefined identifier string
      operationId: create-a-custom-event-with-predefined-identifier-string
      x-api-path-slug: customeventsid-put
      parameters:
      - in: body
        name: body
        description: Custom event resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Custom
      - Event
      - Predefined
      - ID
  /custom-events/{id}/rules:
    get:
      summary: Retrieve a list of rules for custom event
      description: ""
      operationId: ""
      x-api-path-slug: customeventsidrules-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Rulescustom
      - Event
    put:
      summary: Update the rules for custom event
      description: ""
      operationId: ""
      x-api-path-slug: customeventsidrules-put
      parameters:
      - in: body
        name: body
        description: Set of rules resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Rulescustom
      - Event
  /custom-events/{id}/rules/history:
    get:
      summary: Retrieve the change history of the set of rules for a custom event
      description: |-
        Retrieve the change history of the set of rules for the selected custom event.
        The history is updated each time you change the rules.
      operationId: retrieve-the-change-history-of-the-set-of-rules-for-the-selected-custom-event-the-history-is-updated
      x-api-path-slug: customeventsidruleshistory-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Change
      - History
      - Of
      - Set
      - Of
      - Rulesa
      - Custom
      - Event
  /custom-events/{id}/rules/history/{version}:
    get:
      summary: Retrieve the record from the change history of the set of rules for
        a custom event
      description: |-
        Retrieve the record from the change history of the set of rules for the selected custom event.
        A history record is created each time you change the rules.
      operationId: retrieve-the-record-from-the-change-history-of-the-set-of-rules-for-the-selected-custom-event-a-hist
      x-api-path-slug: customeventsidruleshistoryversion-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Record
      - From
      - Change
      - History
      - Of
      - Set
      - Of
      - Rulesa
      - Custom
      - Event
  /custom-events/{id}/rules/versions/{version}:
    get:
      summary: Retrieve the version of the set of rules for a custom event
      description: |-
        Retrieve the version of the selected set of rules for the selected custom event.
        The versions are created each time you change the rules.
      operationId: retrieve-the-version-of-the-selected-set-of-rules-for-the-selected-custom-event-the-versions-are-cre
      x-api-path-slug: customeventsidrulesversionsversion-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Version
      - Of
      - Set
      - Of
      - Rulesa
      - Custom
      - Event
  /events/{eventType}:
    get:
      summary: Retrieve the event information
      description: ""
      operationId: ""
      x-api-path-slug: eventseventtype-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Event
      - Information
  /queue/custom-events/{id}:
    delete:
      summary: Delete a scheduled custom event
      description: Delete a scheduled custom event with predefined identifier string
      operationId: delete-a-scheduled-custom-event-with-predefined-identifier-string
      x-api-path-slug: queuecustomeventsid-delete
      responses:
        200:
          description: OK
      tags:
      - Scheduled
      - Custom
      - Event
    get:
      summary: Retrieve a scheduled custom event
      description: Retrieve a scheduled custom event with predefined identifier string
      operationId: retrieve-a-scheduled-custom-event-with-predefined-identifier-string
      x-api-path-slug: queuecustomeventsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Scheduled
      - Custom
      - Event
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