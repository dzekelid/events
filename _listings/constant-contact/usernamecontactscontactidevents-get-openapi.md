---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Get Per-Contact Campaign Events
  description: Get Per-Contact Campaign Events
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