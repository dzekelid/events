---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List contact events by contact ID
  description: Lists contact events by contact ID. The ID of the contact must be specified.
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