swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 1
info:
  title: ConstantContact
  description: constant-contact-inc-is-an-online-marketing-company-offering-email-marketing-social-media-marketing-online-survey-and-event-marketing-tools-primarily-to-small-businesses-nonprofit-organizations-and-membership-associations-
  termsOfService: http://www.constantcontact.com/uidocs/CCSiteOwnerAgreement.jsp
  version: 1.0.0
host: api.constantcontact.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/campaigns/{campaign-id}/events/:
    get:
      summary: Get Campaign Events
      description: Get Campaign Events
      operationId: get-campaign-events
      x-api-path-slug: usernamecampaignscampaignidevents-get
      parameters:
      - in: path
        name: campaign-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Campaign
      - Events
  /{username}/contacts/{contact-id}/events/:
    get:
      summary: Get Per-Contact Campaign Events
      description: Get Per-Contact Campaign Events
      operationId: get-percontact-campaign-events
      x-api-path-slug: usernamecontactscontactidevents-get
      parameters:
      - in: path
        name: contact-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Per-Contact
      - Campaign
      - Events
  /{username}/events:
    get:
      summary: List Events
      description: List Events
      operationId: list-events
      x-api-path-slug: usernameevents-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
    post:
      summary: Add Event
      description: Add Event
      operationId: add-event
      x-api-path-slug: usernameevents-post
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Event
  /{username}/events/{event-id}:
    get:
      summary: Get Event
      description: Get Event
      operationId: get-event
      x-api-path-slug: usernameeventseventid-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Event