swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 1
info:
  title: IBM Watson Machine Learning API
  description: -authorizationstep-by-step-instruction-how-to-use-watson-machine-learning-servicecan-be-found-herehttpsdatascience-ibm-comdocscontentanalyzedatamloverview-htmlcontextanalytics-ibm-watson-machine-learning-credentialsto-start-working-with-api-one-needs-to-generate-an-access-token-using-the-username-and-passwordavailable-on-the-service-credentials-tab-of-the-ibm-watson-machine-learning-service-instance-or-also-available-in-the-vcap-environment-variable-example-of-the-service-credentialsjson----url-httpsibmwatsonml-mybluemix-net----username-c1ef4b802ee2458eab92e9ca97ec657d----password-030528d45a3e4d4c92585d553513be6f----instance-id-a751c209954edc32b441ad56ce7a9f40example-of-obtaining-access-token-from-token-endpoint-using-http-basic-auth-for-details-please-refer-to-token-section-belowcurl-basic-user-usernamepassword-httpsibmwatsonml-mybluemix-netv3identitytokenthe-obtained-access-token-needs-to-be-prepended-with-bearer-word-and-it-needs-to-be-passed-in-the-authorization-header-for-api-calls-example-of-api-request-with-bearer-access-tokencurl-httpsibmwatsonml-mybluemix-netv3wml-instances00fd89e68cf24712a068ade10277b649published-models-h-authorization-bearer-eyjhbgcioijsuzuxmiisinr5cci6ikpxvcj9-eyj0zw5hbnrjzci6imu4ymqzzgm3lwi5y2utndy1oc1iz----apache-spark-service-credentialsthe-ibm-watson-machine-learning-cooperates-with-the-apache-spark-as-a-service-to-create-batch-stream-deploymentsand-for-learning-configuration-functionality-for-api-methods-requiring-apache-spark-service-instance-a-custom-header-xsparkserviceinstancewith-service-credentials-must-be-specified-the-header-value-is-a-base64-encoded-string-with-the-json-data-containing-service-credentials-and-spark-version-example-of-the-json-data---credentials------tenant-ids068ade10277b6495605b1d10fv12b------tenant-id-full00fd89e68cf24712a068ade10277b649-41f37bf21b954c65a15605b1d10fb12b------cluster-master-urlhttpsspark-bluemix-net------instance-id00fd89e68cf24712a068ade10277b649------tenant-secretc74c37cf482a4da4836ef32ca26ccbb9------planibm-sparkservice-paygopersonal------version2-0
  version: 1.0.0
basePath: v3/
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
host: ibm-watson-ml.mybluemix.net