---
name: Instructure
x-slug: instructure
description: Instructure makes software that makes smarter people. Products include
  Canvas LMS, Bridge and Canvas Network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
x-kinRank: "8"
x-alexaRank: "367"
tags: Events
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/apis.md
specificationVersion: "0.14"
apis:
- name: Instructure Canvas Calendar Events API List calendar events
  x-api-slug: instructure-canvas-calendar-events-api
  description: List calendar events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events
  tags: Calendar,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-events-get-openapi.md
- name: Instructure Canvas Calendar Events API Create a calendar event
  x-api-slug: instructure-canvas-calendar-events-api
  description: Create a calendar event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events
  tags: Calendar,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-events-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-events-post-openapi.md
- name: Instructure Canvas Calendar Events API Delete a calendar event
  x-api-slug: instructure-canvas-calendar-events-api
  description: Delete a calendar event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}
  tags: Calendar,Events,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsid-delete-openapi.md
- name: Instructure Canvas Calendar Events API Get a single calendar event or assignment
  x-api-slug: instructure-canvas-calendar-events-api
  description: Get a single calendar event or assignment.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}
  tags: Calendar,Events,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsid-get-openapi.md
- name: Instructure Canvas Calendar Events API Update a calendar event
  x-api-slug: instructure-canvas-calendar-events-api
  description: Update a calendar event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}
  tags: Calendar,Events,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsid-put-openapi.md
- name: Instructure Canvas Calendar Events API Reserve a time slot
  x-api-slug: instructure-canvas-calendar-events-api
  description: Reserve a time slot.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}/reservations
  tags: Calendar,Events,Id,Reservations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsidreservations-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsidreservations-post-openapi.md
- name: Instructure Canvas Calendar Events API Reserve a time slot
  x-api-slug: instructure-canvas-calendar-events-api
  description: Reserve a time slot.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//calendar_events/{id}/reservations/participant_id
  tags: Calendar,Events,Id,Reservations,Participant,Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsidreservationsparticipant-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/calendar-eventsidreservationsparticipant-id-post-openapi.md
- name: Instructure Canvas Calendar Events API
  x-api-slug: instructure-canvas-calendar-events-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/openapi.md
- name: Instructure Canvas Courses API Retrieve captured events
  x-api-slug: instructure-canvas-courses-api
  description: Retrieve captured events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/{id}/events
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Id,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidevents-get-openapi.md
- name: Instructure Canvas Courses API Submit captured events
  x-api-slug: instructure-canvas-courses-api
  description: Submit captured events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//courses/{course_id}/quizzes/quiz_id/submissions/{id}/events
  tags: Courses,Course,Id,Quizzes,Quiz,Id,Submissions,Id,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidevents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/coursescourse-idquizzesquiz-idsubmissionsidevents-post-openapi.md
- name: Instructure Canvas Courses API
  x-api-slug: instructure-canvas-courses-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/openapi.md
- name: Instructure Canvas Users API List upcoming assignments, calendar events
  x-api-slug: instructure-canvas-users-api
  description: List upcoming assignments, calendar events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/self/upcoming_events
  tags: Users,Self,Upcoming,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/usersselfupcoming-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/usersselfupcoming-events-get-openapi.md
- name: Instructure Canvas Users API List calendar events for a user
  x-api-slug: instructure-canvas-users-api
  description: List calendar events for a user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1//users/{user_id}/calendar_events
  tags: Users,User,Id,Calendar,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/usersuser-idcalendar-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/usersuser-idcalendar-events-get-openapi.md
- name: Instructure Canvas Users API
  x-api-slug: instructure-canvas-users-api
  description: Instructure makes software that makes smarter people. Products include
    Canvas LMS, Bridge and Canvas Network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/820-instructure.jpg
  humanURL: http://instructure.com
  baseURL: https://canvas.instructure.com//api/v1
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/instructure/openapi.md
x-common:
- type: x-blog
  url: http://blog.instructure.com
- type: x-blog-rss
  url: http://voice.instructure.com/CMS/UI/Modules/BizBlogger/rss.aspx?tabid=772438&moduleid=1638884&maxcount=25&t=415c2e5d197a4d6f7cdcc81385b677f1
- type: x-crunchbase
  url: https://crunchbase.com/organization/instructure
- type: x-crunchbase
  url: http://www.crunchbase.com/company/instructure
- type: x-email
  url: info@instructure.com
- type: x-email
  url: jobs@instructure.com
- type: x-email
  url: privacy@instructure.com
- type: x-email
  url: legal@instructure.com
- type: x-github
  url: https://github.com/instructure
- type: x-twitter
  url: https://twitter.com/instructure
- type: x-website
  url: http://instructure.com
- type: x-website
  url: https://canvas.instructure.com/doc/api/index.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---