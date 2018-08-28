---
swagger: "2.0"
x-collection-name: Square
x-complete: 0
info:
  title: Square Connect API Modifies a timecard's details. This creates an API_EDIT
    event for the timecard. You can view a timecard's event history with the List
    Timecard Events endpoint.
  description: Modifies a timecard's details. This creates an API_EDIT event for the
    timecard. You can view a timecard's event history with the List Timecard Events
    endpoint.
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/me/timecards/{timecard_id}:
    put:
      summary: Modifies a timecard's details. This creates an API_EDIT event for the
        timecard. You can view a timecard's event history with the List Timecard Events
        endpoint.
      description: Modifies a timecard's details. This creates an API_EDIT event for
        the timecard. You can view a timecard's event history with the List Timecard
        Events endpoint.
      operationId: UpdateTimecard
      x-api-path-slug: v1metimecardstimecard-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: timecard_id
        description: TThe ID of the timecard to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Timecards
      - Details
      - ""
      - This
      - Creates
      - EDIT
      - Eventthe
      - Timecard
      - ""
      - You
      - Can
      - View
      - Timecards
      - Event
      - History
      - List
      - Timecard
      - Events
      - Endpoint
  /v1/me/timecards/{timecard_id}/events:
    get:
      summary: Provides summary information for all events associated with a particular
        timecard.
      description: Provides summary information for all events associated with a particular
        timecard.
      operationId: ListTimecardEvents
      x-api-path-slug: v1metimecardstimecard-idevents-get
      parameters:
      - in: path
        name: timecard_id
        description: The ID of the timecard to list events for
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Summary
      - Information
      - Events
      - Associated
      - Particular
      - Timecard
  /v1/{location_id}/cash-drawer-shifts/{shift_id}:
    get:
      summary: Provides the details for a single cash drawer shift, including all
        events that occurred during the shift.
      description: Provides the details for a single cash drawer shift, including
        all events that occurred during the shift.
      operationId: RetrieveCashDrawerShift
      x-api-path-slug: v1location-idcashdrawershiftsshift-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the location to list cash drawer shifts for
      - in: path
        name: shift_id
        description: The shifts ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Detailsa
      - Single
      - Cash
      - Drawer
      - Shift
      - ""
      - Including
      - ""
      - Events
      - That
      - Occurred
      - During
      - Shift
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