---
name: Twine
x-slug: twine
description: 'Twine Health is a cloud-based collaborative care platform for chronic
  disease management. It consists of a patient engagement portal, a peer support network,
  a care management solution, and an outcome analytics tool. The platform enables
  users to co-create personalized care plans that serve as common ground for collaboration
  with their care team: their own providers such as physicians and nurse practitioners;
  their family and friends; and coaches such as nurses, pharmacists, health coaches,
  and more.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Events
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/apis.md
specificationVersion: "0.14"
apis:
- name: Twine - List calendar events
  x-api-slug: calendar-event-get
  description: Get a list of calendar events
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-event-get-openapi.md
- name: Twine - Create calendar event
  x-api-slug: calendar-event-post
  description: Create a calendar event for a patient. Attribute `all_day` must be
    set to `true` and `end_at` cannot be set for `plan-check-in` event type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-event-post-openapi.md
- name: Twine - Delete a calendar event
  x-api-slug: calendar-eventid-delete
  description: Delete a calendar event by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-delete-openapi.md
- name: Twine - Get a calendar event
  x-api-slug: calendar-eventid-get
  description: Get a calendar event by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-get-openapi.md
- name: Twine - Update a calendar event
  x-api-slug: calendar-eventid-patch
  description: Update a calendar event for a patient. Attribute `all_day` must be
    true and `end_at` cannot be specified for `plan-check-in` event type. To mark
    a calendar event as 'completed', set `completed_at` and `completed_by` to desired
    values.  To mark a completed calendar event as 'not completed', set `completed_at`
    and `completed_by` to `null`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-patch-openapi.md
- name: Twine - Create calendar event
  x-api-slug: calendar-event-post
  description: Create a calendar event for a patient. Attribute `all_day` must be
    set to `true` and `end_at` cannot be set for `plan-check-in` event type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-event-post-openapi.md
- name: Twine - Delete a calendar event
  x-api-slug: calendar-eventid-delete
  description: Delete a calendar event by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-delete-openapi.md
- name: Twine - Get a calendar event
  x-api-slug: calendar-eventid-get
  description: Get a calendar event by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-get-openapi.md
- name: Twine - Update a calendar event
  x-api-slug: calendar-eventid-patch
  description: Update a calendar event for a patient. Attribute `all_day` must be
    true and `end_at` cannot be specified for `plan-check-in` event type. To mark
    a calendar event as 'completed', set `completed_at` and `completed_by` to desired
    values.  To mark a completed calendar event as 'not completed', set `completed_at`
    and `completed_by` to `null`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-patch-openapi.md
- name: Twine - Update a calendar event
  x-api-slug: calendar-eventid-patch
  description: Update a calendar event for a patient. Attribute `all_day` must be
    true and `end_at` cannot be specified for `plan-check-in` event type. To mark
    a calendar event as 'completed', set `completed_at` and `completed_by` to desired
    values.  To mark a completed calendar event as 'not completed', set `completed_at`
    and `completed_by` to `null`.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-patch-openapi.md
- name: Twine - Get a calendar event
  x-api-slug: calendar-eventid-get
  description: Get a calendar event by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-get-openapi.md
- name: Twine - Delete a calendar event
  x-api-slug: calendar-eventid-delete
  description: Delete a calendar event by id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-eventid-delete-openapi.md
- name: Twine - Create calendar event
  x-api-slug: calendar-event-post
  description: Create a calendar event for a patient. Attribute `all_day` must be
    set to `true` and `end_at` cannot be set for `plan-check-in` event type.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twinehealth.png
  humanURL: http://twinehealth.com
  baseURL: https://api.twinehealth.com//pub
  tags: Wearables, Healthcare, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/twine/calendar-event-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://twilio.api.gallery.streamdata.io
- type: x-api-stack
  url: http://twine.stack.network
- type: x-authentication
  url: http://developer.twinehealth.com/#section/Authentication
- type: x-developer
  url: http://developer.twinehealth.com/
- type: x-website
  url: http://twinehealth.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---