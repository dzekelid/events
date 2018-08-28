---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: IBM Watson IoT Platform Query draft event types
  description: |-
    Event types are used to model the events that are published to the
    Watson IoT Platform.  An event type must be created in an organization
    before more complex processing can be performed on the native event.

    The **/draft/event/types** endpoint returns the list of all of the draft
    event types that have been defined for the organization in the Watson
    IoT Platform.  Various query parameters can be used to filter, sort and
    page through the list of draft event types that are returned.
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
  /event/types/{eventTypeId}:
    get:
      summary: Get an active event type
      description: Retrieve the active event type with the specified id.
      operationId: retrieve-the-active-event-type-with-the-specified-id
      x-api-path-slug: eventtypeseventtypeid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Event
      - Types
      - EventTypeId
  /draft/event/types/{eventTypeId}:
    get:
      summary: Get a draft event type
      description: Retrieve the draft event type with the specified id.
      operationId: retrieve-the-draft-event-type-with-the-specified-id
      x-api-path-slug: drafteventtypeseventtypeid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Event
      - Types
      - EventTypeId
    put:
      summary: Update a draft event type
      description: "Updates the draft event type with the specified id. The following\nproperties
        can be updated:\n\n  - name\n  - description\n  - schemaId\n\nNote that if
        the description field is omitted from the body of the\nupdate, then any existing
        description will be removed from the event\ntype.\n  \nAny changes made to
        the values of the following properties will be\nignored:\n\n  - created\n
        \ - createdBy\n  - updated\n  - updatedBy\n  - refs\n  \nThe values of these
        properties are set on the server as a result of a\nsuccessful update."
      operationId: updates-the-draft-event-type-with-the-specified-id-the-followingproperties-can-be-updated---name---d
      x-api-path-slug: drafteventtypeseventtypeid-put
      parameters:
      - in: body
        name: Event Type
        description: The JSON representation of the event type
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
      - Event
      - Types
      - EventTypeId
    delete:
      summary: Delete a draft event type
      description: "Deletes the draft event type with the specified id from the organization\nin
        the Watson IoT Platform.\n\nPlease note the the delete will fail if the draft
        event type is being \nreferenced by a physical interface."
      operationId: deletes-the-draft-event-type-with-the-specified-id-from-the-organizationin-the-watson-iot-platformpl
      x-api-path-slug: drafteventtypeseventtypeid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Event
      - Types
      - EventTypeId
  /event/types:
    get:
      summary: Query active event types
      description: |-
        Event types are used to model the events that are published to the
        Watson IoT Platform.  An event type must be created in an organization
        before more complex processing can be performed on the native event.

        The **/event/types** endpoint returns the list of all of the active
        event types that have been defined for the organization in the Watson
        IoT Platform.  Various query parameters can be used to filter, sort and
        page through the list of active event types that are returned.
      operationId: event-types-are-used-to-model-the-events-that-are-published-to-thewatson-iot-platform--an-event-type
      x-api-path-slug: eventtypes-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Event
      - Types
  /draft/event/types:
    get:
      summary: Query draft event types
      description: |-
        Event types are used to model the events that are published to the
        Watson IoT Platform.  An event type must be created in an organization
        before more complex processing can be performed on the native event.

        The **/draft/event/types** endpoint returns the list of all of the draft
        event types that have been defined for the organization in the Watson
        IoT Platform.  Various query parameters can be used to filter, sort and
        page through the list of draft event types that are returned.
      operationId: event-types-are-used-to-model-the-events-that-are-published-to-thewatson-iot-platform--an-event-type
      x-api-path-slug: drafteventtypes-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Event
      - Types
    post:
      summary: Create a draft event type
      description: |-
        Creates a new draft event type for the organization in the Watson IoT
        Platform.  The draft event type must reference the schema definition
        that defines the structure of the inbound MQTT event.
      operationId: creates-a-new-draft-event-type-for-the-organization-in-the-watson-iotplatform--the-draft-event-type-
      x-api-path-slug: drafteventtypes-post
      parameters:
      - in: body
        name: Event Type
        description: The JSON representation of the draft event type
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Event
      - Types
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