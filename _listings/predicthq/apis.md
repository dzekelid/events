---
name: PredictHQ
x-slug: predicthq
description: Event visibility yields higher returns & reduces operational costs. PredictHQ
  is the worlds largest source of intelligent event data making businesses smarter.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-developer-predicthq-com.jpg
x-kinRank: "7"
x-alexaRank: "428389"
tags: Events
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/predicthq/apis.md
specificationVersion: "0.14"
apis:
- name: PredictHQ Retrieve Events Calendar
  x-api-slug: predicthq
  description: |-
    This endpoint accepts the same parameters as the ones described in Retrieve All Events and can be used to get a calendar view of all matching events that are available to your account.

    Each day in the calendar contains aggregate counts of all _active_ events for that day.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-developer-predicthq-com.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com////v1/events/calendar/
  tags: Events,Calendar
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/predicthq/v1eventscalendar-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/predicthq/v1eventscalendar-get-openapi.md
- name: PredictHQ Retrieve Events Count
  x-api-slug: predicthq
  description: This endpoint accepts the same parameters as the ones described in
    Retrieve All Events and can be used to get aggregated counts of all matching events
    that are available to your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-developer-predicthq-com.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com////v1/events/count/
  tags: Events,Count
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/predicthq/v1eventscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/predicthq/v1eventscount-get-openapi.md
- name: PredictHQ Retrieve All Events
  x-api-slug: predicthq
  description: Use the below parameters to search and filter all events that are available
    to your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-developer-predicthq-com.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com////v1/events/
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/predicthq/v1events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/predicthq/v1events-get-openapi.md
- name: PredictHQ
  x-api-slug: predicthq
  description: Event visibility yields higher returns & reduces operational costs.
    PredictHQ is the worlds largest source of intelligent event data making businesses
    smarter.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28211-developer-predicthq-com.jpg
  humanURL: http://www.predicthq.com/
  baseURL: https://api.predicthq.com//
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/predicthq/openapi.md
x-common:
- type: x-website
  url: http://www.predicthq.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/predicthq
- type: x-email
  url: support@predicthq.com
- type: x-email
  url: 8Bsupport@predicthq.com
- type: x-email
  url: notices@predicthq.com
- type: x-github
  url: https://github.com/predicthq
- type: x-twitter
  url: https://twitter.com/PredictHQ
- type: x-website
  url: https://developer.predicthq.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---