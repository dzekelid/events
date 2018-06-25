---
name: Getty Images
x-slug: getty-images
description: Find high resolution royalty-free images, editorial stock photos, vector
  art, video footage clips and stock music licensing at the richest image search photo
  library online.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
x-kinRank: "8"
x-alexaRank: "1939"
tags: Events
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/getty-images/apis.md
specificationVersion: "0.14"
apis:
- name: Getty Images Get metadata for multiple events
  x-api-slug: getty-images
  description: "This endpoint returns the detailed event metadata for all specified
    events. Getty Images news, sports and entertainment photographers and\r\nvideographers
    cover editorially relevant events occurring around the world.  All images or video
    clips produced in association with \r\nan event, are assigned the same EventID.
    EventIDs are part of the meta-data returned in SearchForImages Results. Only content
    \r\nproduced under a Getty Images brand name (Getty Images News, Getty Images
    Sports, Getty Images Entertainment, Film Magic, Wire Image) \r\nwill be consistently
    assigned an EventID. The Event framework may also be used to group similar content,
    such as \r\n\"Hats from the Royal Wedding\" or \"Odd-ballOffbeat images of the
    week\". \r\n\r\nYou'll need an API key and access token to use this resource.
    Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
    page for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/events
  tags: Images,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/getty-images/v3events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/getty-images/v3events-get-openapi.md
- name: Getty Images Get metadata for a single event
  x-api-slug: getty-images
  description: "This endpoint returns the detailed event metadata for a specified
    event. Getty Images news, sports and entertainment \r\nphotographers and videographers
    cover editorially relevant events occurring around the world.  \r\nAll images
    or video clips produced in association with an event, are assigned the same EventID.
    \r\nEventIDs are part of the meta-data returned in SearchForImages Results. Only
    content produced under a Getty Images \r\nbrand name (Getty Images News, Getty
    Images Sports, Getty Images Entertainment, Film Magic, Wire Image) will be \r\nconsistently
    assigned an EventID. The Event framework may also be used to group similar content,
    such as \r\n\"Hats from the Royal Wedding\" or \"Odd-ballOffbeat images of the
    week\". \r\n\r\nYou'll need an API key and access token to use this resource.
    Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
    for more information on how to sign up for an API key."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com////v3/events/{id}
  tags: Images,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/getty-images/v3eventsid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/getty-images/v3eventsid-get-openapi.md
- name: Getty Images
  x-api-slug: getty-images
  description: Find high resolution royalty-free images, editorial stock photos, vector
    art, video footage clips and stock music licensing at the richest image search
    photo library online.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1013-getty-images.jpg
  humanURL: http://www.gettyimages.com/
  baseURL: https://api.gettyimages.com//
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/getty-images/openapi.md
x-common:
- type: x-authentication
  url: https://github.com/gettyimages/connect#authentication
- type: x-base
  url: https://connect.gettyimages.com/
- type: x--net-sdk
  url: https://github.com/gettyimages/connect_sdk_csharp
- type: x-crunchbase
  url: https://crunchbase.com/organization/gettyimages
- type: x-crunchbase
  url: http://www.crunchbase.com/company/ge-tt
- type: x-developer
  url: http://api.gettyimages.com/
- type: x-documentation
  url: https://api.gettyimages.com/swagger/ui/index.html
- type: x-email
  url: privacy@gettyimages.com
- type: x-email
  url: sales@gettyimages.com
- type: x-email
  url: copyright@gettyimages.com
- type: x-embeddable
  url: https://github.com/gettyimages/connect#oembed
- type: x-forum
  url: http://api.gettyimages.com/forum
- type: x-getting-started
  url: https://github.com/gettyimages/connect#getting-started
- type: x-github
  url: https://github.com/gettyimages
- type: x-java-sdk
  url: https://github.com/gettyimages/connect_sdk_java
- type: x-node-js-sdk
  url: https://github.com/gettyimages/connect_sdk_nodejs
- type: x-objectivec-sdk
  url: https://github.com/gettyimages/connect_sdk_objective-c
- type: x-php-sdk
  url: https://github.com/gettyimages/connect_sdk_php
- type: x-pricing
  url: http://www.gettyimages.com/subscribe
- type: x-ruby-sdk
  url: https://github.com/gettyimages/connect_sdk_ruby
- type: x-twitter
  url: https://twitter.com/GettyImages
- type: x-website
  url: http://www.gettyimages.com/
- type: x-website
  url: http://gettyimages.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---