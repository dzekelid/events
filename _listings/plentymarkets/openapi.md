swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/contact_events:
    get:
      summary: List contact events
      description: Lists contact events.
      operationId: getRestAccountsContactsContactEvents
      x-api-path-slug: restaccountscontactscontact-events-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Events
    post:
      summary: Create a contact event
      description: Creates a contact event.
      operationId: postRestAccountsContactsContactEvents
      x-api-path-slug: restaccountscontactscontact-events-post
      parameters:
      - in: body
        name: /rest/accounts/contacts/contact_events
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Event
  /rest/accounts/contacts/{contactId}/contact_events:
    get:
      summary: List contact events by contact ID
      description: Lists contact events by contact ID. The ID of the contact must
        be specified.
      operationId: getRestAccountsContactsContactContactEvents
      x-api-path-slug: restaccountscontactscontactidcontact-events-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Events
      - By
      - Contact
      - ID
  /rest/accounts/contacts/contact_events/{contactEventId}:
    delete:
      summary: Delete a contact event
      description: Deletes a contact event. The ID of the contact event must be specified.
      operationId: deleteRestAccountsContactsContactEventsContactevent
      x-api-path-slug: restaccountscontactscontact-eventscontacteventid-delete
      parameters:
      - in: path
        name: contactEventId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Event
    put:
      summary: Update a contact event
      description: Updates a contact event. The ID of the contact event must be specified.
      operationId: putRestAccountsContactsContactEventsContactevent
      x-api-path-slug: restaccountscontactscontact-eventscontacteventid-put
      parameters:
      - in: body
        name: /rest/accounts/contacts/contact_events/{contactEventId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: contactEventId
      responses:
        200:
          description: OK
      tags:
      - Contact
      - Event