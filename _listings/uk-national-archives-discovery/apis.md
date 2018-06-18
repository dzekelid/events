---
name: UK National Archives Discovery
x-slug: uk-national-archives-discovery
description: ""
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Events
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/uk-national-archives-discovery/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Search API Get Events
  x-api-slug: getty-images-search-api
  description: Get metadata for multiple events.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/events
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/uk-national-archives-discovery/v3events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/uk-national-archives-discovery/v3events-get-openapi.md
- name: Getty Images Search API Get Events
  x-api-slug: getty-images-search-api
  description: Get metadata for a single event.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/events/{id}
  tags: Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/uk-national-archives-discovery/v3eventsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/uk-national-archives-discovery/v3eventsid-get-openapi.md
- name: Getty Images Search API Get Search Events
  x-api-slug: getty-images-search-api
  description: Search for events.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com////v3/search/events
  tags: Search,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/uk-national-archives-discovery/v3searchevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/uk-national-archives-discovery/v3searchevents-get-openapi.md
- name: Getty Images Search API
  x-api-slug: getty-images-search-api
  description: Our set of APIs enable seamless integration of Getty Images expansive
    content, powerful search and rich metadata directly into your internal workflows,
    products and services. With Connects API solutions, you can fully control, customize
    and scale as you grow.
  image: ""
  humanURL: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
  baseURL: https://api.gettyimages.com//
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/uk-national-archives-discovery/openapi.md
x-common:
- type: x-website
  url: http://discovery.nationalarchives.gov.uk/SearchUI/api.htm
- type: x-website
  url: http:///Search
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---