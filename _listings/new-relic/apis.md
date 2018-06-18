---
name: New Relic
x-slug: new-relic
description: New Relic???s digital intelligence platform lets developers, ops, and
  tech teams measure and monitor the performance of their applications and infrastructure.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
x-kinRank: "8"
x-alexaRank: "10322"
tags: Events
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Get Alerts Events. Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to list the alert events for your account.\n\nAlerts
    events can be filter by product, target type, group ID, instance ID, and event
    type.\n\nThe options for products are: APM, BROWSER, MOBILE, SERVERS, PLUGINS,
    SYNTHETICS, and ALERTS.\n\nThe options for entity type are: Application, Server,
    KeyTransaction, Plugin, MobileApplication, BrowserApplication, and Monitor.\n\nThe
    options for event type are: NOTIFICATION, DEPLOYMENT, VIOLATION_OPEN, VIOLATION_CLOSE,
    VIOLATION, and INSTRUMENTATION.\n\nThe group ID option is normally the same as
    the entity ID (e.g. an Application group ID and entity ID will be the same), however
    PLUGINS have a group ID representing the PLUGIN itself, and entity IDs for all
    instances of that PLUGIN type.\n\nSee our documentation for a discussion on \noutput
    pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_events.{format}
  tags: Alerts, Events., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/new-relic/alerts-events-format-get-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: New Relic???s digital intelligence platform lets developers, ops, and
    tech teams measure and monitor the performance of their applications and infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/new-relic
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-email
  url: billing@newrelic.com
- type: x-email
  url: resume@newrelic.com
- type: x-email
  url: PR@newrelic.com
- type: x-email
  url: copyright@newrelic.com
- type: x-email
  url: dataprivacy@newrelic.com
- type: x-email
  url: PersonalDataRequest@newrelic.com
- type: x-email
  url: support@newrelic.com
- type: x-email
  url: compliance@newrelic.com
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---