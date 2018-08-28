---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Create a fulfillment event.
  description: Create a fulfillment event..
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/orders/4554953422/events.json:
    get:
      summary: Get all the events from a particular order
      description: Get all the events from a particular order.
      operationId: getAdminOrders4554953422Events.json
      x-api-path-slug: adminorders4554953422events-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Events
      - From
      - Particular
      - Order
  /admin/products/7990943555/events.json:
    get:
      summary: Get all the events from a particular product
      description: Get all the events from a particular product.
      operationId: getAdminProducts7990943555Events.json
      x-api-path-slug: adminproducts7990943555events-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Events
      - From
      - Particular
      - Product
  /admin/events/count.json:
    get:
      summary: Count all the events
      description: Count all the events.
      operationId: getAdminEventsCount.json
      x-api-path-slug: admineventscount-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Count
      - Events
  /admin/orders/4528049998/fulfillments/3770145678/events.json:
    get:
      summary: Get a list of all fulfillment events for a fulfillment
      description: Get a list of all fulfillment events for a fulfillment.
      operationId: getAdminOrders4528049998Fulfillments3770145678Events.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678events-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Fulfillment
      - Eventsa
      - Fulfillment
  /admin/orders/4495703502/fulfillments/3763917198/events/9519874062.json:
    delete:
      summary: Delete a fulfillment event.
      description: Delete a fulfillment event..
      operationId: deleteAdminOrders4495703502Fulfillments3763917198Events9519874062.json
      x-api-path-slug: adminorders4495703502fulfillments3763917198events9519874062-json-delete
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Fulfillment
      - Event
  /admin/orders/4528049998/fulfillments/3770145678/events/#{event_id}.json:
    get:
      summary: Fetch a fulfillment event.
      description: Fetch a fulfillment event..
      operationId: getAdminOrders4528049998Fulfillments3770145678Events#Event.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678eventsevent-id-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: event_id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Fetch
      - Fulfillment
      - Event
  /admin/orders/4495703502/fulfillments/3763917198/events.json:
    post:
      summary: Create a fulfillment event.
      description: Create a fulfillment event..
      operationId: postAdminOrders4495703502Fulfillments3763917198Events.json
      x-api-path-slug: adminorders4495703502fulfillments3763917198events-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Fulfillment
      - Event
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