---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: IBM Watson IoT Platform Get the list of event mappings
  description: |-
    Retrieve the list of event mappings for the draft physical interface.
    Event mappings are keyed off of the event id specified in the MQTT topic
    that the inbound events are published to.
  version: 1.0.0
basePath: /api/v0002
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /physicalinterfaces/{physicalInterfaceId}/events:
    get:
      summary: Get the list of event mappings
      description: |-
        Retrieve the list of event mappings for the active physical interface.
        Event mappings are keyed off of the event id specified in the MQTT topic
        that the inbound events are published to.
      operationId: retrieve-the-list-of-event-mappings-for-the-active-physical-interfaceevent-mappings-are-keyed-off-of
      x-api-path-slug: physicalinterfacesphysicalinterfaceidevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Physicalinterfaces
      - PhysicalInterfaceId
      - Events
  /draft/physicalinterfaces/{physicalInterfaceId}/events:
    get:
      summary: Get the list of event mappings
      description: |-
        Retrieve the list of event mappings for the draft physical interface.
        Event mappings are keyed off of the event id specified in the MQTT topic
        that the inbound events are published to.
      operationId: retrieve-the-list-of-event-mappings-for-the-draft-physical-interfaceevent-mappings-are-keyed-off-of-
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceidevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Physicalinterfaces
      - PhysicalInterfaceId
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