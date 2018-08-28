---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Marks Event List Filter as deleted
  version: 1.0.0
  description: Marks event list filter as deleted.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/group/{id}/events:
    get:
      summary: Get group events by its Id
      description: Get group events by its id.
      operationId: Group_EventsByidBypageSizeBypageNumberBybranchIdByfromBytoBytypeByeventCategoryTypeByactiveRolesOnly
      x-api-path-slug: apigroupidevents-get
      parameters:
      - in: query
        name: activeRolesOnly
        description: Only return active roles
      - in: query
        name: branchId
      - in: query
        name: eventCategoryType
        description: An event category type to return
      - in: query
        name: excludedTypes
        description: Bring back all except these types
      - in: query
        name: from
        description: the date from
      - in: path
        name: id
        description: The id of the group to get events for
      - in: query
        name: includeDrafts
      - in: query
        name: pageNumber
        description: The page of events to return
      - in: query
        name: pageSize
        description: The number of events to return
      - in: query
        name: propertyId
        description: The property the event must relate to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      - in: query
        name: to
        description: the date to
      - in: query
        name: type
        description: The event type to get
      responses:
        200:
          description: OK
      tags:
      - Group
      - Events
      - By
      - Its
      - Id
  /api/property/{id}/events:
    get:
      summary: Get property events by its Id
      description: Get property events by its id.
      operationId: Property_EventsByidBypageSizeBypageNumberBybranchIdByfromBytoBytypeByeventCategoryType
      x-api-path-slug: apipropertyidevents-get
      parameters:
      - in: query
        name: branchId
      - in: query
        name: eventCategoryType
        description: An event category type to return
      - in: query
        name: from
        description: the date from
      - in: path
        name: id
        description: The id of the property to get events for
      - in: query
        name: pageNumber
        description: The page of events to return
      - in: query
        name: pageSize
        description: The number of events to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: to
        description: the date to
      - in: query
        name: type
        description: The event type to get
      responses:
        200:
          description: OK
      tags:
      - Property
      - Events
      - By
      - Its
      - Id
  /api/role/{id}/events:
    get:
      summary: Get role events by its Id
      description: Get role events by its id.
      operationId: Role_EventsByidBypageSizeBypageNumberBybranchIdByfromBytoBytypeByeventCategoryTypeByexcludedTypesByi
      x-api-path-slug: apiroleidevents-get
      parameters:
      - in: query
        name: branchId
      - in: query
        name: eventCategoryType
        description: An event category type to return
      - in: query
        name: excludedTypes
        description: Bring back all except these types
      - in: query
        name: excludeRevised
      - in: query
        name: from
        description: the date from
      - in: path
        name: id
        description: The id of the role to get events for
      - in: query
        name: includeDrafts
      - in: query
        name: pageNumber
        description: The page of events to return
      - in: query
        name: pageSize
        description: The number of events to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: to
        description: the date to
      - in: query
        name: type
        description: The event type to get
      responses:
        200:
          description: OK
      tags:
      - Role
      - Events
      - By
      - Its
      - Id
  /api/sync/mailsync:
    post:
      summary: Syncronise Email with Rezi Events, attach documents etc
      description: Syncronise email with rezi events, attach documents etc.
      operationId: Sync_EmailBymailSyncDataContract
      x-api-path-slug: apisyncmailsync-post
      parameters:
      - in: body
        name: mailSyncDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Syncronise
      - Email
      - Rezi
      - Events
      - ""
      - Attach
      - Documents
      - Etc
  /api/list/event/{id}:
    get:
      summary: Get an EventListDataContract by event Id.
      description: Get an eventlistdatacontract by event id..
      operationId: List_GetByid
      x-api-path-slug: apilisteventid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - EventListDataContract
      - By
      - Event
      - Id
  /api/property/{id}/owners/events:
    get:
      summary: Get property events for the current owner by its Id
      description: Get property events for the current owner by its id.
      operationId: Property_OwnersEventsByidBypageSizeBypageNumberBybranchIdByfromBytoBytypeByeventCategoryType
      x-api-path-slug: apipropertyidownersevents-get
      parameters:
      - in: query
        name: branchId
      - in: query
        name: eventCategoryType
        description: An event category type to return
      - in: query
        name: from
        description: the date from
      - in: path
        name: id
        description: The id of the property to get events for
      - in: query
        name: pageNumber
        description: The page of events to return
      - in: query
        name: pageSize
        description: The number of events to return
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: to
        description: the date to
      - in: query
        name: type
        description: The event type to get
      responses:
        200:
          description: OK
      tags:
      - Property
      - Eventsthe
      - Current
      - Owner
      - By
      - Its
      - Id
  /api/digitalsignature/signable/bounced/{fingerprint}:
    post:
      summary: creates an event when a envelope is bounced by signable
      description: Creates an event when a envelope is bounced by signable.
      operationId: DigitalSignature_BouncedByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablebouncedfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Envelope
      - Is
      - Bounced
      - By
      - Signable
  /api/digitalsignature/signable/opened/{fingerprint}:
    post:
      summary: creates an event when a document is opened
      description: Creates an event when a document is opened.
      operationId: DigitalSignature_OpenedByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignableopenedfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Opened
  /api/digitalsignature/signable/cancelled/{fingerprint}:
    post:
      summary: creates an event when a document is cancelled
      description: Creates an event when a document is cancelled.
      operationId: DigitalSignature_CancelledByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablecancelledfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Cancelled
  /api/digitalsignature/signable/sent/{fingerprint}:
    post:
      summary: creates an event when a document is sent out by signable
      description: Creates an event when a document is sent out by signable.
      operationId: DigitalSignature_SentByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablesentfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Sent
      - Out
      - By
      - Signable
  /api/digitalsignature/signable/signed/{fingerprint}:
    post:
      summary: creates an event when a document is signed
      description: Creates an event when a document is signed.
      operationId: DigitalSignature_SignedByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablesignedfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Signed
  /api/digitalsignature/signable/completed/{fingerprint}:
    post:
      summary: creates an event when a document is completed
      description: Creates an event when a document is completed.
      operationId: DigitalSignature_CompletedByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablecompletedfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Completed
  /api/event/{id}:
    get:
      summary: Get an event by its Id
      description: Get an event by its id.
      operationId: Event_GetByid
      x-api-path-slug: apieventid-get
      parameters:
      - in: path
        name: id
        description: The id of the role to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Event
      - By
      - Its
      - Id
  /api/event/{id}/addnotetoevent:
    post:
      summary: Put - to update a note on an event.
      description: Put - to update a note on an event..
      operationId: Event_AddNoteToEventByidBydataContract
      x-api-path-slug: apieventidaddnotetoevent-post
      parameters:
      - in: body
        name: dataContract
        description: the note text
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the event id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - '-'
      - To
      - Update
      - Note
      - "On"
      - Event
  /api/event/{id}/seteventnote:
    put:
      summary: Put - to update an event note.
      description: Put - to update an event note..
      operationId: Event_UpdateEventNoteByidBynote
      x-api-path-slug: apieventidseteventnote-put
      parameters:
      - in: path
        name: id
        description: the event note id
      - in: query
        name: note
        description: the note text
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - '-'
      - To
      - Update
      - Event
      - Note
  /api/event/{id}/setstatus:
    post:
      summary: Update Status on an event.
      description: Update status on an event..
      operationId: Event_SetStatusByidBydataContract
      x-api-path-slug: apieventidsetstatus-post
      parameters:
      - in: body
        name: dataContract
        description: the note text
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: the event id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Status
      - "On"
      - Event
  /api/event/recordpropertyownercontact:
    post:
      summary: Records an event on the role representing a neg being in contact for
        a property they own
      description: Records an event on the role representing a neg being in contact
        for a property they own.
      operationId: Event_RecordPropertyOwnerContactByrecordPropertyOwnerContactDataContract
      x-api-path-slug: apieventrecordpropertyownercontact-post
      parameters:
      - in: body
        name: recordPropertyOwnerContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contacta
      - Property
      - They
      - Own
  /api/event/recordownercontact:
    post:
      summary: Records an event on the role representing a neg being in contact for
        an owner
      description: Records an event on the role representing a neg being in contact
        for an owner.
      operationId: Event_RecordOwnerContactByrecordOwnerContactDataContract
      x-api-path-slug: apieventrecordownercontact-post
      parameters:
      - in: body
        name: recordOwnerContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contactan
      - Owner
  /api/event/recordenquiry:
    post:
      summary: Records an event on the role representing a neg being in contact with
        a person
      description: Records an event on the role representing a neg being in contact
        with a person.
      operationId: Event_RecordEnquiryByrecordEnquiryDataContract
      x-api-path-slug: apieventrecordenquiry-post
      parameters:
      - in: body
        name: recordEnquiryDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Role
      - Representing
      - Neg
      - Being
      - In
      - Contact
      - Person
  /api/event/{id}/setnegotiators:
    post:
      summary: Changes the negotiators for an event
      description: Changes the negotiators for an event.
      operationId: Event_SetNegotiatorsByidBycommandDataContract
      x-api-path-slug: apieventidsetnegotiators-post
      parameters:
      - in: body
        name: commandDataContract
        description: Command Data Contract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Event Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Negotiatorsan
      - Event
  /api/event/{id}/setowningteam:
    put:
      summary: Changes the owning team of an event
      description: Changes the owning team of an event.
      operationId: Event_SetOwningTeamByidByteamId
      x-api-path-slug: apieventidsetowningteam-put
      parameters:
      - in: path
        name: id
        description: Event Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: Team Id for new owning team
      responses:
        200:
          description: OK
      tags:
      - Changes
      - Owning
      - Team
      - Of
      - Event
  /api/todo/event/savetodo:
    post:
      summary: Save or Updates a Event ToDo and and its tasks
      description: Save or updates a event todo and and its tasks.
      operationId: EventToDo_SaveToDoBytoDoSave
      x-api-path-slug: apitodoeventsavetodo-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: toDoSave
        description: A wrapper for the todo save data and the various data contracts
          needed
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Save
      - S
      - Event
      - ToDo
      - And
      - Its
      - Tasks
  /api/todo/event/addtasks:
    put:
      summary: Add tasks to a Event ToDo
      description: Add tasks to a event todo.
      operationId: EventToDo_AddTasksByaddEventTasksCommandDataContract
      x-api-path-slug: apitodoeventaddtasks-put
      parameters:
      - in: body
        name: addEventTasksCommandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Tasks
      - To
      - Event
      - ToDo
  /api/todo/event/task/{eventId}:
    get:
      summary: Gets all tasks for a particular event / appointment
      description: Gets all tasks for a particular event / appointment.
      operationId: EventToDo_EventTasksByeventIdBypageSizeBypageNumber
      x-api-path-slug: apitodoeventtaskeventid-get
      parameters:
      - in: path
        name: eventId
        description: Id of event or appointment
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page size
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Tasksa
      - Particular
      - Event
      - ""
      - ""
      - Appointment
  /api/todo/event/task/duedate:
    post:
      summary: Updates the due date of an event task
      description: Updates the due date of an event task.
      operationId: EventToDo_UpdateTaskDueDateBycommandDataContract
      x-api-path-slug: apitodoeventtaskduedate-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Due
      - Date
      - Of
      - Event
      - Task
  /api/group/recordcontact:
    post:
      summary: Records an event on the group representing a neg being in contact
      description: Records an event on the group representing a neg being in contact.
      operationId: Group_RecordContactByrecordGroupContactDataContract
      x-api-path-slug: apigrouprecordcontact-post
      parameters:
      - in: body
        name: recordGroupContactDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Records
      - Event
      - "On"
      - Group
      - Representing
      - Neg
      - Being
      - In
      - Contact
  /api/list/events/filters/{id}:
    delete:
      summary: Marks Event List Filter as deleted
      description: Marks event list filter as deleted.
      operationId: List_DeleteEventFilterByid
      x-api-path-slug: apilisteventsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Event
      - List
      - Filter
      - As
      - Deleted
  /api/list/events/csv:
    post:
      summary: Generates a csv file from selected event list items
      description: Generates a csv file from selected event list items.
      operationId: List_GenerateEventCsvBycommandDataContract
      x-api-path-slug: apilisteventscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Event
      - List
      - Items
  /api/negotiator/intervaleventcounts:
    post:
      summary: Return interval based event counts for negotiators.
      description: Return interval based event counts for negotiators..
      operationId: Negotiator_IntervalEventCountsByintervalEventCountDataContract
      x-api-path-slug: apinegotiatorintervaleventcounts-post
      parameters:
      - in: body
        name: intervalEventCountDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - Interval
      - Based
      - Event
      - Countsnegotiators
  /api/people/{id}/redact:
    post:
      summary: "Redact a Person by PersonId\r\nFirst request is just logged as an
        event \r\nSecond request must be by a branch admin and actually redacts the
        person"
      description: "Redact a person by personid\r\nfirst request is just logged as
        an event \r\nsecond request must be by a branch admin and actually redacts
        the person."
      operationId: People_RedactByidBynote
      x-api-path-slug: apipeopleidredact-post
      parameters:
      - in: path
        name: id
      - in: query
        name: note
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Redact
      - Person
      - By
      - "PersonId\r\nFirst"
      - Request
      - Is
      - Just
      - Logged
      - As
      - Event
      - Second
      - Request
      - Must
      - Be
      - By
      - Branch
      - Admin
      - Actually
      - Redacts
      - Person
  /api/role/createreferralevent:
    post:
      summary: Creates a referral event on the role
      description: Creates a referral event on the role.
      operationId: Role_CreateReferralEventByreferralData
      x-api-path-slug: apirolecreatereferralevent-post
      parameters:
      - in: body
        name: referralData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Referral
      - Event
      - "On"
      - Role
  /api/sendgrid/bounce:
    post:
      summary: creates an event when a envelope is bounced by sendgrid
      description: Creates an event when a envelope is bounced by sendgrid.
      operationId: SendGrid_BouncedBybounceData
      x-api-path-slug: apisendgridbounce-post
      parameters:
      - in: body
        name: bounceData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Envelope
      - Is
      - Bounced
      - By
      - Sendgrid
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