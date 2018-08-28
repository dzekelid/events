swagger: "2.0"
x-collection-name: Netatmo
x-complete: 1
info:
  title: Netatmo
  description: we-develop-groundbreaking-intuitive-and-beautifullydesigned-connected-consumer-electronics--truly-smart-our-innovative-products-provide-a-seamless-experience-that-helps-users-create-a-safer-healthier-and-more-comfortable-home---we-carefully-design-the-mechanics-electronics-and-embedded-software-of-all-our-products-to-the-highest-standards--our-mobile-and-web-applications-are-designed-to-be-simple-to-operate-yet-deliver-a-rich-user-experience-
  termsOfService: https://dev.netatmo.com/dev/resources/legal/introduction
  contact:
    name: Netatmo
    email: contact-api@netatmo.com
  version: 1.1.1
host: api.netatmo.net
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /geteventsuntil:
    get:
      summary: Get Geteventsuntil
      description: Returns the snapshot associated to an event.
      operationId: geteventsuntil
      x-api-path-slug: geteventsuntil-get
      parameters:
      - in: query
        name: event_id
        description: Your request will retrieve all the events until this one
      - in: query
        name: home_id
        description: ID of the Home youre interested in
      responses:
        200:
          description: OK
      tags:
      - Events
  /getnextevents:
    get:
      summary: Get Getnextevents
      description: Returns previous events.
      operationId: getnextevents
      x-api-path-slug: getnextevents-get
      parameters:
      - in: query
        name: event_id
        description: Your request will retrieve events occured before this one
      - in: query
        name: home_id
        description: ID of the Home youre interested in
      - in: query
        name: size
        description: Number of events to retrieve
      responses:
        200:
          description: OK
      tags:
      - Devices
      - Events