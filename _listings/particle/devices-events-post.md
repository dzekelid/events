---
swagger: "2.0"
info:
  title: Particle Add Devices Events
  description: Publish an event
  version: 1.0.0
host: api.particle.io
basePath: v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/events:
    post:
      summary: Add Devices Events
      description: Publish an event
      operationId: postDevicesEvents
      parameters:
      - in: formData
        name: data
        description: Event data
      - in: formData
        name: name
        description: Event name
      - in: formData
        name: private
        description: If you wish this event to be publicly visible
      - in: formData
        name: ttl
        description: How long the event should persist
      responses:
        200:
          description: OK
      tags:
      - devices
      - events
definitions:
  AccessTokenInfo:
    properties:
      expires_at:
        description: This is a default description.
        type: delete
      client:
        description: This is a default description.
        type: delete
  DeviceInfo:
    properties:
      name:
        description: This is a default description.
        type: delete
      last_app:
        description: This is a default description.
        type: delete
      last_ip_address:
        description: This is a default description.
        type: delete
      last_heard:
        description: This is a default description.
        type: delete
      connected:
        description: This is a default description.
        type: delete
      last_iccid:
        description: This is a default description.
        type: delete
      imei:
        description: This is a default description.
        type: delete
x-collection-name: Particle
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