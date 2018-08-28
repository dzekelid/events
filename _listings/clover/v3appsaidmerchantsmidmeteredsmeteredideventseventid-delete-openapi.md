---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Delete an app billing metered event, if not charged.
  version: 1.0.0
  description: This deletes an app billing metered event, if the event has not been
    charged yet. See https://docs.clover.com/launch/billing/ for more information.
    Requires an OAuth generated token.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/cash_events:
    get:
      summary: Get all cash events
      description: Retrieve all cash events for this merchant. Cash events can also
        be consumed by registering a Webhook callback. See https://docs.clover.com/build/webhooks/
      operationId: GetAllCashEvents
      x-api-path-slug: v3merchantsmidcash-events-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [employee, device]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Cash
      - Events
  /v3/merchants/{mId}/employees/{empId}/cash_events:
    get:
      summary: Get all cash events for an employee
      description: Retrieve cash events filtered by employee ID. Cash events can also
        be consumed by registering a Webhook callback. See https://docs.clover.com/build/webhooks/
      operationId: GetEmployeeCashEvents
      x-api-path-slug: v3merchantsmidemployeesempidcash-events-get
      parameters:
      - in: path
        name: empId
        description: Employee Id
      - in: query
        name: expand
        description: 'Expandable fields: [employee, device]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Employees
      - EmpId
      - Cash
      - Events
  /v3/merchants/{mId}/devices/{deviceId}/cash_events:
    get:
      summary: Get all cash events for a device
      description: Retrieve cash events filtered by device ID. Cash events can also
        be consumed by registering a Webhook callback. See https://docs.clover.com/build/webhooks/
      operationId: GetDeviceCashEvents
      x-api-path-slug: v3merchantsmiddevicesdeviceidcash-events-get
      parameters:
      - in: path
        name: deviceId
        description: Device Id
      - in: query
        name: expand
        description: 'Expandable fields: [employee, device]'
      - in: query
        name: filter
        description: 'Filter fields: [employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Devices
      - DeviceId
      - Cash
      - Events
  /v3/apps/{aId}/merchants/{mId}/metereds/{meteredId}/events/{eventId}:
    get:
      summary: Get an app billing metered event
      description: This enables you to fetch the details on a merchants app billing
        metered event. Requires an OAuth generated token.
      operationId: GetMerchantAppMeteredEvent
      x-api-path-slug: v3appsaidmerchantsmidmeteredsmeteredideventseventid-get
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: path
        name: eventId
      - in: path
        name: meteredId
        description: Metered Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Metereds
      - MeteredId
      - Events
      - EventId
    delete:
      summary: Delete an app billing metered event, if not charged.
      description: This deletes an app billing metered event, if the event has not
        been charged yet. See https://docs.clover.com/launch/billing/ for more information.
        Requires an OAuth generated token.
      operationId: DeleteMerchantAppMeteredEvent
      x-api-path-slug: v3appsaidmerchantsmidmeteredsmeteredideventseventid-delete
      parameters:
      - in: path
        name: aId
        description: App Id
      - in: path
        name: eventId
      - in: path
        name: meteredId
        description: Metered Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Apps
      - Merchants
      - Metereds
      - MeteredId
      - Events
      - EventId
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