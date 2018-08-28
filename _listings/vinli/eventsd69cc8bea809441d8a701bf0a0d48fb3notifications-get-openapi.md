---
swagger: "2.0"
x-collection-name: Vinli
x-complete: 0
info:
  title: Vinli Get Notifications for an Event
  description: Get notifications for an event.
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/62976d30-b6dc-40f1-8422-ccc367572101/events:
    get:
      summary: Get All Events for a Device
      description: Get all events for a device.
      operationId: Devices62976d30B6dc40f18422Ccc367572101EventsGet
      x-api-path-slug: devices62976d30b6dc40f18422ccc367572101events-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Eventsa
      - Device
  /events/1caa8fff-c9be-4506-bcb8-38371c25aa14:
    get:
      summary: Get a Specific Event
      description: Get a specific event.
      operationId: Events1caa8fffC9be4506Bcb838371c25aa14Get
      x-api-path-slug: events1caa8fffc9be4506bcb838371c25aa14-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Specific
      - Event
  /events/d69cc8be-a809-441d-8a70-1bf0a0d48fb3/notifications:
    get:
      summary: Get Notifications for an Event
      description: Get notifications for an event.
      operationId: EventsD69cc8beA809441d8a701bf0a0d48fb3NotificationsGet
      x-api-path-slug: eventsd69cc8bea809441d8a701bf0a0d48fb3notifications-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Notificationsan
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