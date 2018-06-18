---
name: IBM Watson
x-slug: ibm-watson
description: Meet IBM Watson, a cognitive system that enables a new partnership between
  people and computers that enhances and scales human expertise. Watson has been learning
  the language of professions and is trained by experts to work across many different
  industries.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Events
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/ibm-watson/apis.md
specificationVersion: "0.14"
apis:
- name: IBM Watson IoT Platform Get the list of event mappings
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the list of event mappings for the active physical interface.
    Event mappings are keyed off of the event id specified in the MQTT topic
    that the inbound events are published to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//physicalinterfaces/{physicalInterfaceId}/events
  tags: Internet of Things,Physicalinterfaces,PhysicalInterfaceId,Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/ibm-watson/physicalinterfacesphysicalinterfaceidevents-get-openapi.md
- name: IBM Watson IoT Platform Get the list of event mappings
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Retrieve the list of event mappings for the draft physical interface.
    Event mappings are keyed off of the event id specified in the MQTT topic
    that the inbound events are published to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}/events
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceidevents-get-openapi.md
- name: IBM Watson IoT Platform Map an event to the draft physical interface
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Maps an event id to a specific event type for the draft specified
    physical interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}/events
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId,Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceidevents-post-openapi.md
- name: IBM Watson IoT Platform Remove an event mapping from the draft physical interface
  x-api-slug: ibm-watson-iot-platform
  description: |-
    Removes the event mapping with the specified id from the draft physical
    interface.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002//draft/physicalinterfaces/{physicalInterfaceId}/events/{eventId}
  tags: Internet of Things,Draft,Physicalinterfaces,PhysicalInterfaceId,Events,EventId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/ibm-watson/draftphysicalinterfacesphysicalinterfaceideventseventid-delete-openapi.md
- name: IBM Watson IoT Platform
  x-api-slug: ibm-watson-iot-platform
  description: Meet IBM Watson, a cognitive system that enables a new partnership
    between people and computers that enhances and scales human expertise. Watson
    has been learning the language of professions and is trained by experts to work
    across many different industries.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ibm-watson-logo.png
  humanURL: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
  baseURL: https:////api/v0002
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/ibm-watson/openapi.md
x-common:
- type: x-application-gallery
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/gallery.html
- type: x-blog
  url: https://developer.ibm.com/watson/blog/
- type: x-blog-rss
  url: https://developer.ibm.com/watson/feed/
- type: x-developer
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/doc/
- type: x-developer
  url: https://developer.ibm.com/watson/
- type: x-documentation
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/apis/
- type: x-forum
  url: https://developer.ibm.com/answers/smartspace/watson/
- type: x-getting-started
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/getstarted.html
- type: x-github
  url: https://github.com/IBM-Watson
- type: x-partners
  url: http://www.ibm.com/smarterplanet/us/en/ibmwatson/ecosystem.html
- type: x-privacy
  url: http://www.ibm.com/privacy/us/en/?lnk=flg-priv-usen
- type: x-terms-of-service
  url: http://www.ibm.com/legal/us/en/?lnk=flg-tous-usen
- type: x-twitter
  url: https://twitter.com/IBMWatson
- type: x-videos
  url: http://www.ibm.com/smarterplanet/us/en/ibmwatson/
- type: x-website
  url: https://www.ibm.com/smarterplanet/us/en/ibmwatson/developercloud/
- type: x-white-papers
  url: https://developer.ibm.com/watson/docs/whitepapers/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---