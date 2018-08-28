---
name: Box
x-slug: box
description: Box is changing how you manage content across your business from simple
  file sharing to building custom apps.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
x-kinRank: "9"
x-alexaRank: "445"
tags: Events
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/box/apis.md
specificationVersion: "0.14"
apis:
- name: Box User Events, Enterprise Events
  x-api-slug: box
  description: |-
    Use this to get events for a given user. A chunk of event objects is returned for the user based on the parameters passed in. Parameters indicating how many chunks are left as well as the next stream_position are also returned.

    To retrieve Enterprise Events specify 'stream_type=admin_logs'. Retrieves up to a year' events for all users in an enterprise. Upper and lower bounds as well as filters can be applied to the results.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//events
  tags: Documents,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/box/events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/box/events-get-openapi.md
- name: Box Long polling
  x-api-slug: box
  description: "To get real-time notification of activity in a Box account, use the
    long poll feature of the /events API. To do so, first call the /events API with
    an OPTIONS call to retrieve the long poll URL to use. Next, make a GET request
    to the provided URL to begin listening for events. If an event occurs within an
    account you are monitoring, you will receive a response with the value new_change.
    It\u2019s important to note that this response will not come with any other details,
    but should serve as a prompt to take further action such as calling the /events
    endpoint with your last known stream_position. After sending this response, the
    server will close the connection and you will need to repeat the long poll process
    to begin listening for events again.\nIf no events occur for a period of time
    after you make the GET request to the long poll URL, you will receive a response
    with the value reconnect. When you receive this response, you\u2019ll make another
    OPTIONS call to the /events endpoint and repeat the long poll process.\nIf you
    receive no events in retry_timeout seconds, you should make another GET request
    to the real time server (i.e. URL in the response). This might be necessary in
    case you do not receive the reconnect message in the face of network errors.\nIf
    you receive max_retries error when making GET requests to the real time server,
    you should make another OPTIONS request."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0//events
  tags: Documents,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/box/events-options-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/box/events-options-openapi.md
- name: Box
  x-api-slug: box
  description: Box.net provides a sophisticated API for their online document sharing
    and collaboration web application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/162-box.jpg
  humanURL: http://box.com
  baseURL: https://api.box.com//2.0
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/box/openapi.md
x-common:
- type: x-base
  url: https://api.box.com/
- type: x-blog
  url: http://blog.box.com/
- type: x-blog-rss
  url: http://blog.box.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/box
- type: x-crunchbase
  url: https://crunchbase.com/organization/box
- type: x-developer
  url: http://developers.box.com
- type: x-github
  url: https://github.com/boxdotnet
- type: x-pricing
  url: https://developers.box.com/box-platform-pricing/
- type: x-road-map
  url: https://developers.box.com/roadmap/
- type: x-twitter
  url: https://twitter.com/BoxPlatform
- type: x-twitter
  url: https://twitter.com/BoxHQ
- type: x-website
  url: http://box.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---