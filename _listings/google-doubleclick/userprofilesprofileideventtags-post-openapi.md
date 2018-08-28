---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Insert Event Tag
  version: 1.0.0
  description: Inserts a new event tag.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/eventTags:
    get:
      summary: Get Event Tags
      description: Retrieves a list of event tags, possibly filtered.
      operationId: dfareporting.eventTags.list
      x-api-path-slug: userprofilesprofileideventtags-get
      parameters:
      - in: query
        name: adId
        description: Select only event tags that belong to this ad
      - in: query
        name: advertiserId
        description: Select only event tags that belong to this advertiser
      - in: query
        name: campaignId
        description: Select only event tags that belong to this campaign
      - in: query
        name: definitionsOnly
        description: Examine only the specified campaign or advertisers event tags
          for matching selector criteria
      - in: query
        name: enabled
        description: Select only enabled event tags
      - in: query
        name: eventTagTypes
        description: Select only event tags with the specified event tag types
      - in: query
        name: ids
        description: Select only event tags with these IDs
      - in: path
        name: profileId
        description: User profile ID associated with this request
      - in: query
        name: searchString
        description: Allows searching for objects by name or ID
      - in: query
        name: sortField
        description: Field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is ASCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
    patch:
      summary: Update Event Tag
      description: Updates an existing event tag. This method supports patch semantics.
      operationId: dfareporting.eventTags.patch
      x-api-path-slug: userprofilesprofileideventtags-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: id
        description: Event tag ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
    post:
      summary: Insert Event Tag
      description: Inserts a new event tag.
      operationId: dfareporting.eventTags.insert
      x-api-path-slug: userprofilesprofileideventtags-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
    put:
      summary: Update Event Tag
      description: Updates an existing event tag.
      operationId: dfareporting.eventTags.update
      x-api-path-slug: userprofilesprofileideventtags-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
  /userprofiles/{profileId}/eventTags/{id}:
    delete:
      summary: Delete Event Tag
      description: Deletes an existing event tag.
      operationId: dfareporting.eventTags.delete
      x-api-path-slug: userprofilesprofileideventtagsid-delete
      parameters:
      - in: path
        name: id
        description: Event tag ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
    get:
      summary: Get Event Tag
      description: Gets one event tag by ID.
      operationId: dfareporting.eventTags.get
      x-api-path-slug: userprofilesprofileideventtagsid-get
      parameters:
      - in: path
        name: id
        description: Event tag ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Event Tag
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---