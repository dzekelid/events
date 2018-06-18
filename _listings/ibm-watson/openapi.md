---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 1
info:
  title: IBM Watson IoT Platform HTTP REST API
  description: the-information-management-capabilities-of-ibm-watson-iot-platform-helpyou-to-organize-and-integrate-data-coming-in-to-and-going-out-of-watson-iotplatform---with-these-apis-you-will-be-able-to---work-with-device-state-regardless-of-whether-the-actual-device-on-online----or-offline----provide-your-application-developers-with-consistent-interfaces-to-access----eventdriven-device-data-in-a-restlike-manner----normalize-data-from-devices-of-different-makes-or-models-that-publish----data-in-different-formatsfor-information-on-how-to-use-watson-iot-platform-apis-generally-see-the-api-documentationhttpsconsole-ng-bluemix-netdocsservicesiotreferenceapi-html-for-more-general-information-on-how-to-use-watson-iot-platform-seethe-general-documentationhttpsconsole-ng-bluemix-netdocsservicesiotindex-htmlgettingstartedtemplate
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
    post:
      summary: Map an event to the draft physical interface
      description: |-
        Maps an event id to a specific event type for the draft specified
        physical interface.
      operationId: maps-an-event-id-to-a-specific-event-type-for-the-draft-specifiedphysical-interface
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceidevents-post
      parameters:
      - in: body
        name: Event Mapping
        description: The JSON representation of the event mapping
        schema:
          $ref: '#/definitions/holder'
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
  /draft/physicalinterfaces/{physicalInterfaceId}/events/{eventId}:
    delete:
      summary: Remove an event mapping from the draft physical interface
      description: |-
        Removes the event mapping with the specified id from the draft physical
        interface.
      operationId: removes-the-event-mapping-with-the-specified-id-from-the-draft-physicalinterface
      x-api-path-slug: draftphysicalinterfacesphysicalinterfaceideventseventid-delete
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
      - EventId
---