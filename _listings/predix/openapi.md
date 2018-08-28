swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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
          description: OK
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
  /v1/tenants/{tenant_uuid}/events/{uuid}:
    get:
      summary: Get Tenants Events
      description: Get tenants events.
      operationId: getV1TenantsTenantUuEventsUu
      x-api-path-slug: v1tenantstenant-uuideventsuuid-get
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Events
    put:
      summary: Put Tenants Events
      description: Put tenants events.
      operationId: putV1TenantsTenantUuEventsUu
      x-api-path-slug: v1tenantstenant-uuideventsuuid-put
      parameters:
      - in: body
        name: event
        description: event
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Events
    delete:
      summary: Delete Tenants Events
      description: Delete tenants events.
      operationId: deleteV1TenantsTenantUuEventsUu
      x-api-path-slug: v1tenantstenant-uuideventsuuid-delete
      parameters:
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      - in: path
        name: uuid
        description: uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Events
  /v1/tenants/{tenant_uuid}/event-search:
    get:
      summary: Get Tenants Event Search
      description: Get tenants event search.
      operationId: getV1TenantsTenantUuEventSearch
      x-api-path-slug: v1tenantstenant-uuideventsearch-get
      parameters:
      - in: query
        name: query
        description: query
      - in: path
        name: tenant_uuid
        description: tenant_uuid
      responses:
        200:
          description: Successful response
      tags:
      - Tenants
      - Event
      - Search