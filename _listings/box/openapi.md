---
swagger: "2.0"
x-collection-name: Box
x-complete: 1
info:
  title: Box
  description: the-box-content-api-gives-you-access-to-secure-content-management-and-content-experience-features-for-use-in-your-own-app--it-strives-to-be-restful-and-is-organized-around-the-main-resources-youre-familiar-with-from-the-box-web-interface-
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    get:
      summary: User Events, Enterprise Events
      description: |-
        Use this to get events for a given user. A chunk of event objects is returned for the user based on the parameters passed in. Parameters indicating how many chunks are left as well as the next stream_position are also returned.

        To retrieve Enterprise Events specify 'stream_type=admin_logs'. Retrieves up to a year' events for all users in an enterprise. Upper and lower bounds as well as filters can be applied to the results.
      operationId: getUserEvents
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: created_after
        description: A lower bound on the timestamp of the events returned
      - in: query
        name: created_before
        description: An upper bound on the timestamp of the events returned
      - in: query
        name: event_type
        description: A comma-separated list of events to filter by
      - in: query
        name: limit
        description: Limits the number of events returned
      - in: query
        name: stream_position
        description: The location in the event stream at which you want to start receiving
          events
      - in: query
        name: stream_type
        description: 'Limits the type of events returned: all: returns everything,
          changes: returns tree changes, sync: returns tree changes only for sync
          folders'
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Events
    options:
      summary: Long polling
      description: "To get real-time notification of activity in a Box account, use
        the long poll feature of the /events API. To do so, first call the /events
        API with an OPTIONS call to retrieve the long poll URL to use. Next, make
        a GET request to the provided URL to begin listening for events. If an event
        occurs within an account you are monitoring, you will receive a response with
        the value new_change. It\u2019s important to note that this response will
        not come with any other details, but should serve as a prompt to take further
        action such as calling the /events endpoint with your last known stream_position.
        After sending this response, the server will close the connection and you
        will need to repeat the long poll process to begin listening for events again.\nIf
        no events occur for a period of time after you make the GET request to the
        long poll URL, you will receive a response with the value reconnect. When
        you receive this response, you\u2019ll make another OPTIONS call to the /events
        endpoint and repeat the long poll process.\nIf you receive no events in retry_timeout
        seconds, you should make another GET request to the real time server (i.e.
        URL in the response). This might be necessary in case you do not receive the
        reconnect message in the face of network errors.\nIf you receive max_retries
        error when making GET requests to the real time server, you should make another
        OPTIONS request."
      operationId: eventLongPolling
      x-api-path-slug: events-options
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Events
---