---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Event Eventid Photo
  version: 1.0.0
  description: Post event eventid photo.
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
  /api/v1/admin/event/approve/{eventId}:
    post:
      summary: Post Admin Event Approve Eventid
      description: Post admin event approve eventid.
      operationId: postApiV1AdminEventApproveEvent
      x-api-path-slug: apiv1admineventapproveeventid-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Approve
      - Eventid
  /api/v1/admin/event/{eventId}/thumbnail/url:
    post:
      summary: Post Admin Event Eventid Thumbnail Url
      description: Post admin event eventid thumbnail url.
      operationId: postApiV1AdminEventEventThumbnailUrl
      x-api-path-slug: apiv1admineventeventidthumbnailurl-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: body
        name: url
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Eventid
      - Thumbnail
      - Url
  /api/v1/art/invited/{artistId}/{eventId}:
    get:
      summary: Get Art Invited Artistid Eventid
      description: Get art invited artistid eventid.
      operationId: getApiV1ArtInvitedArtistEvent
      x-api-path-slug: apiv1artinvitedartistideventid-get
      parameters:
      - in: path
        name: artistId
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Art
      - Invited
      - Artistid
      - Eventid
  /api/v1/event/sales/{eventId}/start:
    post:
      summary: Post Event Sales Eventid Start
      description: Post event sales eventid start.
      operationId: postApiV1EventSalesEventStart
      x-api-path-slug: apiv1eventsaleseventidstart-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Sales
      - Eventid
      - Start
  /api/v1/event/sales/{eventId}/stop:
    post:
      summary: Post Event Sales Eventid Stop
      description: Post event sales eventid stop.
      operationId: postApiV1EventSalesEventStop
      x-api-path-slug: apiv1eventsaleseventidstop-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Sales
      - Eventid
      - Stop
  /api/v1/event/banner/{eventId}:
    post:
      summary: Post Event Banner Eventid
      description: Post event banner eventid.
      operationId: postApiV1EventBannerEvent
      x-api-path-slug: apiv1eventbannereventid-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Event
      - Banner
      - Eventid
    delete:
      summary: Delete Event Banner Eventid
      description: Delete event banner eventid.
      operationId: deleteApiV1EventBannerEvent
      x-api-path-slug: apiv1eventbannereventid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Banner
      - Eventid
  /api/v1/event/promo/{eventId}:
    post:
      summary: Post Event Promo Eventid
      description: Post event promo eventid.
      operationId: postApiV1EventPromoEvent
      x-api-path-slug: apiv1eventpromoeventid-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Event
      - Promo
      - Eventid
    delete:
      summary: Delete Event Promo Eventid
      description: Delete event promo eventid.
      operationId: deleteApiV1EventPromoEvent
      x-api-path-slug: apiv1eventpromoeventid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Promo
      - Eventid
  /api/v1/event/{eventId}/video:
    post:
      summary: Post Event Eventid Veo
      description: Post event eventid veo.
      operationId: postApiV1EventEventVeo
      x-api-path-slug: apiv1eventeventidvideo-post
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: body
        name: url
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Veo
  /api/v1/event/{eventId}/video/{videoId}:
    delete:
      summary: Delete Event Eventid Veo Veoid
      description: Delete event eventid veo veoid.
      operationId: deleteApiV1EventEventVeoVeo
      x-api-path-slug: apiv1eventeventidvideovideoid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: path
        name: videoId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Veo
      - Veoid
  /api/v1/event/{eventId}/photo:
    post:
      summary: Post Event Eventid Photo
      description: Post event eventid photo.
      operationId: postApiV1EventEventPhoto
      x-api-path-slug: apiv1eventeventidphoto-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Photo
  /api/v1/event/{eventId}/photos:
    post:
      summary: Post Event Eventid Photos
      description: Post event eventid photos.
      operationId: postApiV1EventEventPhotos
      x-api-path-slug: apiv1eventeventidphotos-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Photos
  /api/v1/event/{eventId}/photo/{photoId}:
    delete:
      summary: Delete Event Eventid Photo Photoid
      description: Delete event eventid photo photoid.
      operationId: deleteApiV1EventEventPhotoPhoto
      x-api-path-slug: apiv1eventeventidphotophotoid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: path
        name: photoId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Photo
      - Photoid
  /api/v1/event/{eventId}/partner:
    post:
      summary: Post Event Eventid Partner
      description: Post event eventid partner.
      operationId: postApiV1EventEventPartner
      x-api-path-slug: apiv1eventeventidpartner-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Partner
    delete:
      summary: Delete Event Eventid Partner
      description: Delete event eventid partner.
      operationId: deleteApiV1EventEventPartner
      x-api-path-slug: apiv1eventeventidpartner-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Event
      - Eventid
      - Partner
  /api/v1/gigme/event/{eventId}/related:
    get:
      summary: Get Gigme Event Eventid Related
      description: Get gigme event eventid related.
      operationId: getApiV1GigmeEventEventRelated
      x-api-path-slug: apiv1gigmeeventeventidrelated-get
      parameters:
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Eventid
      - Related
  /api/v1/gigme/event/{eventId}/like:
    get:
      summary: Get Gigme Event Eventid Like
      description: Get gigme event eventid like.
      operationId: getApiV1GigmeEventEventLike
      x-api-path-slug: apiv1gigmeeventeventidlike-get
      parameters:
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Eventid
      - Like
  /api/v1/gigme/event/{eventId}/dislike:
    get:
      summary: Get Gigme Event Eventid Dislike
      description: Get gigme event eventid dislike.
      operationId: getApiV1GigmeEventEventDislike
      x-api-path-slug: apiv1gigmeeventeventiddislike-get
      parameters:
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Eventid
      - Dislike
  /api/v1/rating/{eventId}/artists:
    get:
      summary: Get Rating Eventid Artists
      description: Get rating eventid artists.
      operationId: getApiV1RatingEventArtists
      x-api-path-slug: apiv1ratingeventidartists-get
      parameters:
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Rating
      - Eventid
      - Artists
  /api/v1/ticket/{eventId}/{ticketId}:
    delete:
      summary: Delete Ticket Eventid Ticketid
      description: Delete ticket eventid ticketid.
      operationId: deleteApiV1TicketEventTicket
      x-api-path-slug: apiv1ticketeventidticketid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: path
        name: ticketId
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Eventid
      - Ticketid
  /api/v1/ticket/{eventId}:
    get:
      summary: Get Ticket Eventid
      description: Get ticket eventid.
      operationId: getApiV1TicketEvent
      x-api-path-slug: apiv1ticketeventid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: query
        name: from
      - in: query
        name: to
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Eventid
  /api/v1/ticket/{eventId}/export:
    get:
      summary: Get Ticket Eventid Export
      description: Get ticket eventid export.
      operationId: getApiV1TicketEventExport
      x-api-path-slug: apiv1ticketeventidexport-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: eventId
      - in: query
        name: from
      - in: query
        name: to
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Eventid
      - Export
  /api/v1/admin/event/{page}:
    get:
      summary: Get Admin Event Page
      description: Get admin event page.
      operationId: getApiV1AdminEventPage
      x-api-path-slug: apiv1admineventpage-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: page
      - in: query
        name: request.cityId
      - in: query
        name: request.from
      - in: query
        name: request.isRecommended
      - in: query
        name: request.placeId
      - in: query
        name: request.placeName
      - in: query
        name: request.query
      - in: query
        name: request.status
      - in: query
        name: request.to
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Page
  /api/v1/admin/event/reject:
    post:
      summary: Post Admin Event Reject
      description: Post admin event reject.
      operationId: postApiV1AdminEventReject
      x-api-path-slug: apiv1admineventreject-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Reject
  /api/v1/admin/event/defer:
    post:
      summary: Post Admin Event Defer
      description: Post admin event defer.
      operationId: postApiV1AdminEventDefer
      x-api-path-slug: apiv1admineventdefer-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Defer
  /api/v1/admin/event/add:
    post:
      summary: Post Admin Event Add
      description: Post admin event add.
      operationId: postApiV1AdminEventAdd
      x-api-path-slug: apiv1admineventadd-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: event
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
  /api/v1/admin/event/tags/main:
    get:
      summary: Get Admin Event Tags Main
      description: Get admin event tags main.
      operationId: getApiV1AdminEventTagsMain
      x-api-path-slug: apiv1admineventtagsmain-get
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Tags
      - Main
  /api/v1/admin/event/tags/additional:
    get:
      summary: Get Admin Event Tags Additional
      description: Get admin event tags additional.
      operationId: getApiV1AdminEventTagsAdditional
      x-api-path-slug: apiv1admineventtagsadditional-get
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Tags
      - Itional
  /api/v1/admin/event/{primaryId}/merge/{secondaryId}:
    get:
      summary: Get Admin Event Primaryid Merge Secondaryid
      description: Get admin event primaryid merge secondaryid.
      operationId: getApiV1AdminEventPrimaryMergeSecondary
      x-api-path-slug: apiv1admineventprimaryidmergesecondaryid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: primaryId
      - in: path
        name: secondaryId
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Primaryid
      - Merge
      - Secondaryid
  /api/v1/admin/event/statistic:
    get:
      summary: Get Admin Event Statistic
      description: Get admin event statistic.
      operationId: getApiV1AdminEventStatistic
      x-api-path-slug: apiv1admineventstatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Event
      - Statistic
  /api/v1/event/{id}/details:
    get:
      summary: Get Event Details
      description: Get event details.
      operationId: getApiV1EventDetails
      x-api-path-slug: apiv1eventiddetails-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Event
      - Details
  /api/v1/event/{unique}/details:
    get:
      summary: Get Event Unique Details
      description: Get event unique details.
      operationId: getApiV1EventUniqueDetails
      x-api-path-slug: apiv1eventuniquedetails-get
      parameters:
      - in: path
        name: unique
      responses:
        200:
          description: OK
      tags:
      - Event
      - Unique
      - Details
  /api/v1/event/{id}:
    get:
      summary: Get Event
      description: Get event.
      operationId: getApiV1Event
      x-api-path-slug: apiv1eventid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Event
  /api/v1/event/active:
    get:
      summary: Get Event Active
      description: Get event active.
      operationId: getApiV1EventActive
      x-api-path-slug: apiv1eventactive-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Event
      - Active
  /api/v1/event/past:
    get:
      summary: Get Event Past
      description: Get event past.
      operationId: getApiV1EventPast
      x-api-path-slug: apiv1eventpast-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Event
      - Past
  /api/v1/event/add:
    post:
      summary: Post Event Add
      description: Post event add.
      operationId: postApiV1EventAdd
      x-api-path-slug: apiv1eventadd-post
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Event
  /api/v1/event/del/{id}:
    delete:
      summary: Delete Event Del
      description: Delete event del.
      operationId: deleteApiV1EventDel
      x-api-path-slug: apiv1eventdelid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Event
      - Del
  /api/v1/event/save:
    post:
      summary: Post Event Save
      description: Post event save.
      operationId: postApiV1EventSave
      x-api-path-slug: apiv1eventsave-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        description: ','
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Event
      - Save
  /api/v1/event/add/private:
    post:
      summary: Post Event Add Private
      description: Post event add private.
      operationId: postApiV1EventAddPrivate
      x-api-path-slug: apiv1eventaddprivate-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        description: ','
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Event
      - ""
      - Private
  /api/v1/gigme/event/previews/{page}:
    post:
      summary: Post Gigme Event Previews Page
      description: Post gigme event previews page.
      operationId: postApiV1GigmeEventPreviewsPage
      x-api-path-slug: apiv1gigmeeventpreviewspage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: preview
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Previews
      - Page
  /api/v1/gigme/event/{page}:
    post:
      summary: Post Gigme Event Page
      description: Post gigme event page.
      operationId: postApiV1GigmeEventPage
      x-api-path-slug: apiv1gigmeeventpage-post
      parameters:
      - in: path
        name: page
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Page
  /api/v1/gigme/event/previews/map:
    post:
      summary: Post Gigme Event Previews Map
      description: Post gigme event previews map.
      operationId: postApiV1GigmeEventPreviewsMap
      x-api-path-slug: apiv1gigmeeventpreviewsmap-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Previews
      - Map
  /api/v1/gigme/event/history:
    get:
      summary: Get Gigme Event History
      description: Get gigme event history.
      operationId: getApiV1GigmeEventHistory
      x-api-path-slug: apiv1gigmeeventhistory-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - History
  /api/v1/gigme/event/recommended:
    get:
      summary: Get Gigme Event Recommended
      description: Get gigme event recommended.
      operationId: getApiV1GigmeEventRecommended
      x-api-path-slug: apiv1gigmeeventrecommended-get
      parameters:
      - in: query
        name: request.amount
      - in: query
        name: request.dateFilter
      - in: query
        name: request.type
        description: Type of Preview (event or place)
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Recommended
  /api/v1/gigme/event/{placeId}/upcoming:
    get:
      summary: Get Gigme Event Placeid Upcoming
      description: Get gigme event placeid upcoming.
      operationId: getApiV1GigmeEventPlaceUpcoming
      x-api-path-slug: apiv1gigmeeventplaceidupcoming-get
      parameters:
      - in: path
        name: placeId
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Placeid
      - Upcoming
  /api/v1/gigme/event/{id}/details:
    get:
      summary: Get Gigme Event Details
      description: Get gigme event details.
      operationId: getApiV1GigmeEventDetails
      x-api-path-slug: apiv1gigmeeventiddetails-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Details
  /api/v1/gigme/event/{unique}/details:
    get:
      summary: Get Gigme Event Unique Details
      description: Get gigme event unique details.
      operationId: getApiV1GigmeEventUniqueDetails
      x-api-path-slug: apiv1gigmeeventuniquedetails-get
      parameters:
      - in: path
        name: unique
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - Unique
      - Details
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