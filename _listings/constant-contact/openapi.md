---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 1
info:
  title: Constant Contact
  description: make-constant-contacts-leading-email-and-event-marketing-services-accessible-directly-from-your-app-
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
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
---