---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Event Audit Trail Post Tenants Events
  description: Post tenants events.
  version: 1.0.0
host: event-audit-trail.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/plugins/archive/tenants/{tenant_uuid}/staged-events:
    get:
      summary: Get Plugins Archive Tenants Staged Events
      description: Get plugins archive tenants staged events.
      operationId: getV1PluginsArchiveTenantsTenantUuStagedEvents
      x-api-path-slug: v1pluginsarchivetenantstenant-uuidstagedevents-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Plugins
      - Archive
      - Tenants
      - Staged
      - Events
  /v1/tenants/{tenant_uuid}/events:
    get:
      summary: Get Tenants Events
      description: Get tenants events.
      operationId: getV1TenantsTenantUuEvents
      x-api-path-slug: v1tenantstenant-uuidevents-get
      parameters:
      - in: query
        name: classification
        description: classification
      - in: query
        name: context
        description: context
      - in: query
        name: end_date
        description: end_date
      - in: query
        name: start_date
        description: start_date
      - in: query
        name: tag
        description: tag
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Events
    post:
      summary: Post Tenants Events
      description: Post tenants events.
      operationId: postV1TenantsTenantUuEvents
      x-api-path-slug: v1tenantstenant-uuidevents-post
      parameters:
      - in: body
        name: events
        description: events
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
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