swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/art/{id}/events/past:
    get:
      summary: Get Art Events Past
      description: Get art events past.
      operationId: getApiV1ArtEventsPast
      x-api-path-slug: apiv1artideventspast-get
      parameters:
      - in: path
        name: id
        description: Id
      responses:
        200:
          description: OK
      tags:
      - Art
      - Events
      - Past
  /api/v1/city/events:
    get:
      summary: Get City Events
      description: Get city events.
      operationId: getApiV1CityEvents
      x-api-path-slug: apiv1cityevents-get
      responses:
        200:
          description: OK
      tags:
      - City
      - Events
  /api/v1/gigme/artist/{id}/events/future:
    get:
      summary: Get Gigme Artist Events Future
      description: Get gigme artist events future.
      operationId: getApiV1GigmeArtistEventsFuture
      x-api-path-slug: apiv1gigmeartistideventsfuture-get
      parameters:
      - in: path
        name: id
        description: Id
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Artist
      - Events
      - Future
  /api/v1/gigme/artist/{id}/events/past:
    get:
      summary: Get Gigme Artist Events Past
      description: Get gigme artist events past.
      operationId: getApiV1GigmeArtistEventsPast
      x-api-path-slug: apiv1gigmeartistideventspast-get
      parameters:
      - in: path
        name: id
        description: Id
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Artist
      - Events
      - Past
  /api/v1/gigme/city/events:
    get:
      summary: Get Gigme City Events
      description: Get gigme city events.
      operationId: getApiV1GigmeCityEvents
      x-api-path-slug: apiv1gigmecityevents-get
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - City
      - Events