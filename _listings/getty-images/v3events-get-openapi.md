---
swagger: "2.0"
x-collection-name: Getty Images
x-complete: 0
info:
  title: Getty Images Get metadata for multiple events
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
  version: 1.0.0
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/events:
    get:
      summary: Get metadata for multiple events
      description: "This endpoint returns the detailed event metadata for all specified
        events. Getty Images news, sports and entertainment photographers and\r\nvideographers
        cover editorially relevant events occurring around the world.  All images
        or video clips produced in association with \r\nan event, are assigned the
        same EventID. EventIDs are part of the meta-data returned in SearchForImages
        Results. Only content \r\nproduced under a Getty Images brand name (Getty
        Images News, Getty Images Sports, Getty Images Entertainment, Film Magic,
        Wire Image) \r\nwill be consistently assigned an EventID. The Event framework
        may also be used to group similar content, such as \r\n\"Hats from the Royal
        Wedding\" or \"Odd-ballOffbeat images of the week\". \r\n\r\nYou'll need an
        API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key."
      operationId: Events_GetBatch
      x-api-path-slug: v3events-get
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: query
        name: fields
        description: A comma separated list of fields to return in the response
      - in: query
        name: ids
        description: A comma separated list of event ids
      responses:
        200:
          description: OK
      tags:
      - Images
      - Events
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