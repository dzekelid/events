swagger: "2.0"
x-collection-name: Getty Images
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
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
  /v3/events/{id}:
    get:
      summary: Get metadata for a single event
      description: "This endpoint returns the detailed event metadata for a specified
        event. Getty Images news, sports and entertainment \r\nphotographers and videographers
        cover editorially relevant events occurring around the world.  \r\nAll images
        or video clips produced in association with an event, are assigned the same
        EventID. \r\nEventIDs are part of the meta-data returned in SearchForImages
        Results. Only content produced under a Getty Images \r\nbrand name (Getty
        Images News, Getty Images Sports, Getty Images Entertainment, Film Magic,
        Wire Image) will be \r\nconsistently assigned an EventID. The Event framework
        may also be used to group similar content, such as \r\n\"Hats from the Royal
        Wedding\" or \"Odd-ballOffbeat images of the week\". \r\n\r\nYou'll need an
        API key and access token to use this resource. Please see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)\r\npage
        for more information on how to sign up for an API key."
      operationId: Events_Get
      x-api-path-slug: v3eventsid-get
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
      - in: path
        name: id
        description: An event id
      responses:
        200:
          description: OK
      tags:
      - Images
      - Events