---
name: Microsoft Graph
x-slug: microsoft-graph
description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
  cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
  Graph simplifies queries that would otherwise be more complex. You can use Microsoft
  Graph to: Access data from multiple Microsoft cloud services, including Azure Active
  Directory, Exchange Online as part of Office 365, SharePoint, OneDrive, OneNote,
  and Planner. Navigate between entities and relationships. Access intelligence and
  insights from the Microsoft cloud (for commercial users).'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Events
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/apis.md
specificationVersion: "0.14"
apis:
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of events in a calendar.  The list contains
    single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendar/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/mecalendarevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of events in a calendar.  The list contains
    single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendar/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/usersid--userprincipalnamecalendarevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of event objects.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/calendar/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/groupsidcalendarevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of events in a calendar.  The list contains
    single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendars/{id}/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/mecalendarsidevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of events in a calendar.  The list contains
    single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendars/{id}/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/usersid--userprincipalnamecalendarsidevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of events in a calendar.  The list contains
    single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendarGroup/calendars/{id}/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/mecalendargroupcalendarsidevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of events in a calendar.  The list contains
    single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/usersid--userprincipalnamecalendargroupcalendarsidevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of events in a calendar.  The list contains
    single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////me/calendarGroups/{id}/calendars/{id}/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/mecalendargroupsidcalendarsidevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of events in a calendar.  The list contains
    single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/usersid--userprincipalnamecalendargroupsidcalendarsidevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Retrieve a list of event objects.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////groups/{id}/events
  tags: List, Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/groupsidevents-get-openapi.md
- name: Microsoft Graph List Events
  x-api-slug: microsoft-graph
  description: List events Get a list of event objects in the user's mailbox. The
    list contains single instance meetings and series masters.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com////users/{id | userPrincipalName}/events
  tags: List, Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/usersid--userprincipalnameevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/usersid--userprincipalnameevents-get-openapi.md
- name: Microsoft Graph
  x-api-slug: microsoft-graph
  description: 'Microsoft Graph exposes multiple APIs from Office 365 and other Microsoft
    cloud services through a single endpoint: https://graph.microsoft.com. Microsoft
    Graph simplifies queries that would otherwise be more complex. You can use Microsoft
    Graph to: Access data from multiple Microsoft cloud services, including Azure
    Active Directory, Exchange Online as part of Office 365, SharePoint, OneDrive,
    OneNote, and Planner. Navigate between entities and relationships. Access intelligence
    and insights from the Microsoft cloud (for commercial users).'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/microsoft-graph.png
  humanURL: https://developer.microsoft.com/en-us/graph/
  baseURL: https://graph.microsoft.com//
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/microsoft-graph/openapi.md
x-common:
- type: x-change-loge
  url: https://developer.microsoft.com/en-us/graph/docs/overview/changelog
- type: x-documentation
  url: https://developer.microsoft.com/en-us/graph/docs
- type: x-explorer
  url: https://developer.microsoft.com/en-us/graph/graph-explorer
- type: x-getting-started
  url: https://developer.microsoft.com/en-us/graph/docs/get-started/rest
- type: x-github
  url: https://github.com/microsoftgraph
- type: x-sdk
  url: https://developer.microsoft.com/en-us/graph/code-samples-and-sdks
- type: x-website
  url: https://developer.microsoft.com/en-us/graph/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---