swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /schedule/data/events:
    get:
      summary: Generates the calendar that we draw events on
      description: ""
      operationId: scheduleCalendarData
      x-api-path-slug: scheduledataevents-get
      parameters:
      - in: formData
        name: displayGroupIds
        description: The DisplayGroupIds to return the schedule for
      - in: formData
        name: from
        description: From Date Timestamp in Microseconds
      - in: formData
        name: to
        description: To Date Timestamp in Microseconds
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Calendar
      - That
      - We
      - Draw
      - Events
      - "On"
  /schedule/{displayGroupId}/events:
    get:
      summary: Event List
      description: ""
      operationId: scheduleCalendarData
      x-api-path-slug: scheduledisplaygroupidevents-get
      parameters:
      - in: formData
        name: date
        description: Date in Y-m-d H:i:s
      - in: path
        name: displayGroupId
        description: The DisplayGroupId to return the event list for
      responses:
        200:
          description: OK
      tags:
      - Event
      - List
  /schedule:
    post:
      summary: Add Schedule Event
      description: Add a new scheduled event for a Campaign/Layout to be shown on
        a Display Group/Display.
      operationId: scheduleAdd
      x-api-path-slug: schedule-post
      parameters:
      - in: formData
        name: campaignId
        description: The Campaign ID to use for this Event
      - in: formData
        name: commandId
        description: The Command ID to use for this Event
      - in: formData
        name: dayPartId
        description: The Day Part for this event
      - in: formData
        name: displayGroupIds
        description: The Display Group IDs for this event
      - in: formData
        name: displayOrder
        description: The display order for this event
      - in: formData
        name: eventTypeId
        description: The Event Type Id to use for this Event
      - in: formData
        name: fromDt
        description: The from date for this event
      - in: formData
        name: isPriority
        description: An integer indicating the priority of this event
      - in: formData
        name: recurrenceDetail
        description: The interval for the recurrence
      - in: formData
        name: recurrenceRange
        description: The end date for this events recurrence
      - in: formData
        name: recurrenceRepeatsOn
        description: The days of the week that this event repeats - weekly only
      - in: formData
        name: recurrenceType
        description: The type of recurrence to apply to this event
      - in: formData
        name: syncTimezone
        description: Should this schedule be synced to the resulting Display timezone?
      - in: formData
        name: toDt
        description: The to date for this event
      responses:
        200:
          description: OK
      tags:
      - Schedule
      - Event
  /schedule/{eventId}:
    put:
      summary: Edit Schedule Event
      description: Edit a scheduled event for a Campaign/Layout to be shown on a Display
        Group/Display.
      operationId: scheduleEdit
      x-api-path-slug: scheduleeventid-put
      parameters:
      - in: formData
        name: campaignId
        description: The Campaign ID to use for this Event
      - in: formData
        name: commandId
        description: The Command ID to use for this Event
      - in: formData
        name: dayPartId
        description: The Day Part for this event
      - in: formData
        name: displayGroupIds
        description: The Display Group IDs for this event
      - in: formData
        name: displayOrder
        description: The display order for this event
      - in: path
        name: eventId
        description: The Scheduled Event ID
      - in: formData
        name: eventTypeId
        description: The Event Type Id to use for this Event
      - in: formData
        name: fromDt
        description: The from date for this event
      - in: formData
        name: isPriority
        description: An integer indicating the priority of this event
      - in: formData
        name: recurrenceDetail
        description: The interval for the recurrence
      - in: formData
        name: recurrenceRange
        description: The end date for this events recurrence
      - in: formData
        name: recurrenceRepeatsOn
        description: The days of the week that this event repeats - weekly only
      - in: formData
        name: recurrenceType
        description: The type of recurrence to apply to this event
      - in: formData
        name: syncTimezone
        description: Should this schedule be synced to the resulting Display timezone?
      - in: formData
        name: toDt
        description: The to date for this event
      responses:
        200:
          description: OK
      tags:
      - Edit
      - Schedule
      - Event
    delete:
      summary: Delete Event
      description: Delete a Scheduled Event
      operationId: scheduleDelete
      x-api-path-slug: scheduleeventid-delete
      parameters:
      - in: path
        name: eventId
        description: The Scheduled Event ID
      responses:
        200:
          description: OK
      tags:
      - Event