---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Users API List calendar events for a user
  description: List calendar events for a user.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calendar_events:
    get:
      summary: List calendar events
      description: List calendar events.
      operationId: list-calendar-events
      x-api-path-slug: calendar-events-get
      parameters:
      - in: query
        name: all_events
        description: Defaults to false (uses start_date, end_date, and undated criteria)
      - in: query
        name: context_codes[]
        description: List of context codes of courses/groups/users whose events you
          want to see
      - in: query
        name: end_date
        description: Only return events before the end_date (inclusive)
      - in: query
        name: excludes[]
        description: Array of attributes to exclude
      - in: query
        name: start_date
        description: Only return events since the start_date (inclusive)
      - in: query
        name: type
        description: 'Defaults to u201ceventu201dnn        n        n          Allowed
          values: event, assignment'
      - in: query
        name: undated
        description: Defaults to false (dated events only)
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
    post:
      summary: Create a calendar event
      description: Create a calendar event.
      operationId: create-a-calendar-event
      x-api-path-slug: calendar-events-post
      parameters:
      - in: query
        name: calendar_event[child_event_data][X][context_code]
        description: Context code(s) corresponding to the section-level start and
          end time(s)
      - in: query
        name: calendar_event[child_event_data][X][end_at]
        description: Section-level end time(s) if this is a course event
      - in: query
        name: calendar_event[child_event_data][X][start_at]
        description: Section-level start time(s) if this is a course event
      - in: query
        name: calendar_event[context_code]
        description: Context code of the course/group/user whose calendar this event
          should benadded to
      - in: query
        name: calendar_event[description]
        description: Longer HTML description of the event
      - in: query
        name: calendar_event[duplicate][append_iterator]
        description: Defaults to false
      - in: query
        name: calendar_event[duplicate][count]
        description: Number of times to copy/duplicate the event
      - in: query
        name: calendar_event[duplicate][frequency]
        description: Defaults to u201cweeklyu201d
      - in: query
        name: calendar_event[duplicate][interval]
        description: Defaults to 1 if duplicate `count` is set
      - in: query
        name: calendar_event[end_at]
        description: End date/time of the event
      - in: query
        name: calendar_event[location_address]
        description: Location address
      - in: query
        name: calendar_event[location_name]
        description: Location name of the event
      - in: query
        name: calendar_event[start_at]
        description: Start date/time of the event
      - in: query
        name: calendar_event[time_zone_edited]
        description: Time zone of the user editing the event
      - in: query
        name: calendar_event[title]
        description: Short title for the calendar event
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
  /calendar_events/{id}:
    delete:
      summary: Delete a calendar event
      description: Delete a calendar event.
      operationId: delete-a-calendar-event
      x-api-path-slug: calendar-eventsid-delete
      parameters:
      - in: query
        name: cancel_reason
        description: Reason for deleting/canceling the event
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
    get:
      summary: Get a single calendar event or assignment
      description: Get a single calendar event or assignment.
      operationId: get-a-single-calendar-event-or-assignment
      x-api-path-slug: calendar-eventsid-get
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
    put:
      summary: Update a calendar event
      description: Update a calendar event.
      operationId: update-a-calendar-event
      x-api-path-slug: calendar-eventsid-put
      parameters:
      - in: query
        name: calendar_event[child_event_data][X][context_code]
        description: Context code(s) corresponding to the section-level start and
          end time(s)
      - in: query
        name: calendar_event[child_event_data][X][end_at]
        description: Section-level end time(s) if this is a course event
      - in: query
        name: calendar_event[child_event_data][X][start_at]
        description: Section-level start time(s) if this is a course event
      - in: query
        name: calendar_event[context_code]
        description: Context code of the course/group/user whose calendar this event
          should benadded to
      - in: query
        name: calendar_event[description]
        description: Longer HTML description of the event
      - in: query
        name: calendar_event[end_at]
        description: End date/time of the event
      - in: query
        name: calendar_event[location_address]
        description: Location address
      - in: query
        name: calendar_event[location_name]
        description: Location name of the event
      - in: query
        name: calendar_event[start_at]
        description: Start date/time of the event
      - in: query
        name: calendar_event[time_zone_edited]
        description: Time zone of the user editing the event
      - in: query
        name: calendar_event[title]
        description: Short title for the calendar event
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
  /calendar_events/{id}/reservations:
    post:
      summary: Reserve a time slot
      description: Reserve a time slot.
      operationId: reserve-a-time-slot
      x-api-path-slug: calendar-eventsidreservations-post
      parameters:
      - in: query
        name: cancel_existing
        description: Defaults to false
      - in: query
        name: comments
        description: Comments to associate with this reservation
      - in: query
        name: participant_id
        description: User or group id for whom you are making the reservation (depends
          on thenparticipant type)
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
      - Reservations
  /calendar_events/{id}/reservations/participant_id:
    post:
      summary: Reserve a time slot
      description: Reserve a time slot.
      operationId: reserve-a-time-slot
      x-api-path-slug: calendar-eventsidreservationsparticipant-id-post
      parameters:
      - in: query
        name: cancel_existing
        description: Defaults to false
      - in: query
        name: comments
        description: Comments to associate with this reservation
      - in: query
        name: participant_id
        description: User or group id for whom you are making the reservation (depends
          on thenparticipant type)
      responses:
        200:
          description: OK
      tags:
      - Calendar
      - Events
      - Id
      - Reservations
      - Participant
      - Id
  /courses/{course_id}/quizzes/quiz_id/submissions/{id}/events:
    get:
      summary: Retrieve captured events
      description: Retrieve captured events.
      operationId: retrieve-captured-events
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsidevents-get
      parameters:
      - in: query
        name: attempt
        description: The specific submission attempt to look up the events for
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
      - Events
    post:
      summary: Submit captured events
      description: Submit captured events.
      operationId: submit-captured-events
      x-api-path-slug: coursescourse-idquizzesquiz-idsubmissionsidevents-post
      parameters:
      - in: query
        name: quiz_submission_events[]
        description: The submission events to be recorded
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Quizzes
      - Quiz
      - Id
      - Submissions
      - Id
      - Events
  /users/self/upcoming_events:
    get:
      summary: List upcoming assignments, calendar events
      description: List upcoming assignments, calendar events.
      operationId: list-upcoming-assignments-calendar-events
      x-api-path-slug: usersselfupcoming-events-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Self
      - Upcoming
      - Events
  /users/{user_id}/calendar_events:
    get:
      summary: List calendar events for a user
      description: List calendar events for a user.
      operationId: list-calendar-events-for-a-user
      x-api-path-slug: usersuser-idcalendar-events-get
      parameters:
      - in: query
        name: all_events
        description: Defaults to false (uses start_date, end_date, and undated criteria)
      - in: query
        name: context_codes[]
        description: List of context codes of courses/groups/users whose events you
          want to see
      - in: query
        name: end_date
        description: Only return events before the end_date (inclusive)
      - in: query
        name: excludes[]
        description: Array of attributes to exclude
      - in: query
        name: start_date
        description: Only return events since the start_date (inclusive)
      - in: query
        name: type
        description: 'Defaults to u201ceventu201dnn        n        n          Allowed
          values: event, assignment'
      - in: query
        name: undated
        description: Defaults to false (dated events only)
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Id
      - Calendar
      - Events
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