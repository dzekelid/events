---
name: Meetup
description: Meetup is an online social networking portal that facilitates offline
  group meetings in various localities around the world. Meetup allows members to
  find and join groups unified by a common interest, such as politics, books, games,
  movies, health, pets, careers or hobbies.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Meetup-Logo-1-med1.jpg
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Stack
- My API Stack
- Meetups
- Media
- Events
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/meetup/apis.yaml
specificationVersion: "0.14"
apis:
- name: Meetup
  description: Meetup is an online social networking portal that facilitates offline
    group meetings in various localities around the world
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Meetup-Logo-1-med1.jpg
  humanURL: ""
  baseURL: https://api.meetup.com//
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/meetup/urlname-events-get.md
- name: Meetup OpenEvents
  description: Searches for recent and upcoming public events hosted by Meetup groups.
    Its search window  is the past one month through the next three months, and is
    subject to change. Open Events is optimized to search for current events by location,
    category, topic, or text, and only lists Meetups that have **3 or more RSVPs**.
    The number or results returned with each request is not guaranteed to be the same
    as the page size due to secondary filtering. If you're looking for a particular
    event or events within a particular group, use the standard [Events](/meetup_api/docs/2/events/)
    method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Meetup-Logo-1-med1.jpg
  humanURL: http://www.meetup.com/
  baseURL: https://api.meetup.com//
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/meetup/2-open-events-get.md
x-common:
- type: x-base
  url: http://api.meetup.com
- type: x-developer
  url: http://www.meetup.com/meetup_api/
- type: x-github
  url: https://github.com/meetup
- type: x-pricing
  url: http://www.meetup.com/pricing/
- type: x-privacy
  url: http://www.meetup.com/privacy/
- type: x-support
  url: http://www.meetup.com/help/
- type: x-terms-of-service
  url: http://www.meetup.com/terms/
- type: x-twitter
  url: https://twitter.com/MeetupAPI
- type: x-website
  url: http://www.meetup.com/
- type: x-base
  url: http://api.meetup.com
- type: x-developer
  url: http://www.meetup.com/meetup_api/
- type: x-github
  url: https://github.com/meetup
- type: x-pricing
  url: http://www.meetup.com/pricing/
- type: x-privacy
  url: http://www.meetup.com/privacy/
- type: x-support
  url: http://www.meetup.com/help/
- type: x-terms-of-service
  url: http://www.meetup.com/terms/
- type: x-twitter
  url: https://twitter.com/MeetupAPI
- type: x-website
  url: http://www.meetup.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---