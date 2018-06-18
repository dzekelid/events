---
name: Square
x-slug: square
description: Square helps millions of sellers run their business- from secure credit
  card processing to point of sale solutions. Get paid faster with Square and sign
  up today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
x-kinRank: "9"
x-alexaRank: "2436"
tags: Events
created: "2018-06-18"
modified: "2018-06-18"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API Modifies a timecard's details. This creates an API_EDIT
    event for the timecard. You can view a timecard's event history with the List
    Timecard Events endpoint.
  x-api-slug: square-connect-api
  description: Modifies a timecard's details. This creates an API_EDIT event for the
    timecard. You can view a timecard's event history with the List Timecard Events
    endpoint.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/me/timecards/{timecard_id}
  tags: Modifies,Timecards,Details,,This,Creates,EDIT,Eventthe,Timecard,,You,Can,View,Timecards,Event,History,List,Timecard,Events,Endpoint
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/square/v1metimecardstimecard-id-put-openapi.md
- name: Square Connect API Provides summary information for all events associated
    with a particular timecard.
  x-api-slug: square-connect-api
  description: Provides summary information for all events associated with a particular
    timecard.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/me/timecards/{timecard_id}/events
  tags: Provides,Summary,Information,Events,Associated,Particular,Timecard
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/square/v1metimecardstimecard-idevents-get-openapi.md
- name: Square Connect API Provides the details for a single cash drawer shift, including
    all events that occurred during the shift.
  x-api-slug: square-connect-api
  description: Provides the details for a single cash drawer shift, including all
    events that occurred during the shift.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/{location_id}/cash-drawer-shifts/{shift_id}
  tags: Provides,Detailsa,Single,Cash,Drawer,Shift,,Including,,Events,That,Occurred,During,Shift
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/square/v1location-idcashdrawershiftsshift-id-get-openapi.md
- name: Square Connect API
  x-api-slug: square-connect-api
  description: Square helps millions of sellers run their business- from secure credit
    card processing to point of sale solutions. Get paid faster with Square and sign
    up today!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com//
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/square/openapi.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-crunchbase
  url: https://crunchbase.com/organization/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-email
  url: press@squareup.com
- type: x-email
  url: security@squareup.com
- type: x-email
  url: lawenforcement@squareup.com
- type: x-email
  url: redemption@squareup.com
- type: x-email
  url: privacy@squareup.com
- type: x-email
  url: community@squareup.com
- type: x-email
  url: noreply@messaging.squareup.com
- type: x-email
  url: ir@squareup.com
- type: x-email
  url: takedowns@squareup.com
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: http://squareup.com
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---