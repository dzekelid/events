---
name: Lota Data
x-slug: lota-data
description: ""
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Events
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/lota-data/apis.md
specificationVersion: "0.14"
apis:
- name: Lota Data - Get Events
  x-api-slug: events-get
  description: Find event occurrences in the area. returns results at specific place
    and time, event groups are expanded for every occurrence..
  image: ""
  humanURL: http://lotadata.com
  baseURL: https://api2.lotadata.com//v2
  tags: Data, Analysis, API Provider, Profiles, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/lota-data/events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/lota-data/events-get-openapi.md
- name: Lota Data - Get Events
  x-api-slug: eventsid-get
  description: Get specific event details..
  image: ""
  humanURL: http://lotadata.com
  baseURL: https://api2.lotadata.com//v2
  tags: Data, Analysis, API Provider, Profiles, General Data, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/lota-data/eventsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/lota-data/eventsid-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://logmein.api.gallery.streamdata.io
- type: x-api-stack
  url: http://lota.data.stack.network
- type: x-blog
  url: https://www.lotadata.com/blog/
- type: x-developer
  url: https://docs.lotadata.com/
- type: x-documentation
  url: https://docs.lotadata.com/apis.html
- type: x-monetization
  url: https://docs.lotadata.com/monetization.html
- type: x-website
  url: http://lotadata.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---