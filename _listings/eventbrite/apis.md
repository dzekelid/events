---
name: Eventbrite
x-slug: eventbrite
description: Eventbrite brings people together through live experiences. Discover
  events that match your passions, or create your own with online ticketing tools.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
x-kinRank: "9"
x-alexaRank: "643"
tags: Events
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/apis.md
specificationVersion: "0.14"
apis:
- name: Eventbrite - Post Events
  x-api-slug: events-post
  description: Makes a new event, and returns an event for the specified event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/events-post-openapi.md
- name: Eventbrite - Get Events
  x-api-slug: eventsid-get
  description: Returns an event for the specified event. Many of Eventbrite?s API
    use cases resolve around pulling details of a specific event within an Eventbrite
    account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsid-get-openapi.md
- name: Eventbrite - Post Events
  x-api-slug: eventsid-post
  description: Updates an event. Returns an event for the specified event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsid-post-openapi.md
- name: Eventbrite - Get Events Event Checkout Settings
  x-api-slug: eventsevent-idcheckout-settings-get
  description: Gets and returns a list of checkout_settings associated with a given
    event by its event_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idcheckout-settings-get-openapi.md
- name: Eventbrite - Post Events Event Checkout Settings
  x-api-slug: eventsevent-idcheckout-settings-post
  description: Associate a single or set of checkout_settings with a given event by
    its event_id. This does not add more checkout settings to the event, but instead
    replaces all checkout settings for the event with the one(s) submitted. The JSON
    post body is a string list of the checkout_settings IDs you want to associate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idcheckout-settings-post-openapi.md
- name: Eventbrite - Get Events Event Payout Settings
  x-api-slug: eventsevent-idpayout-settings-get
  description: Gets and returns the payout_settings (user instrument ID) associated
    with a given event by its event_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idpayout-settings-get-openapi.md
- name: Eventbrite - Post Events Event Payout Settings
  x-api-slug: eventsevent-idpayout-settings-post
  description: Associate a payout user instrument ID with a given event, or clear
    the association by passing a null value for the user instrument ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idpayout-settings-post-openapi.md
- name: Eventbrite - Get Events
  x-api-slug: eventsid-get
  description: |-
    Returns an event for the specified event. Many of Eventbrite???s API use cases revolve around pulling details
    of a specific event within an Eventbrite account. Does not support fetching a repeating event series parent
    (see GET /series/:id/).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsid-get-openapi.md
- name: Eventbrite - Post Events
  x-api-slug: eventsid-post
  description: |-
    Updates an event. Returns an event for the specified event. Does not support updating a repeating event
    series parent (see POST /series/:id/).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsid-post-openapi.md
- name: Eventbrite - Post Events Publish
  x-api-slug: eventsidpublish-post
  description: |-
    Publishes an event if it has not already been deleted. In order for publish to be permitted, the event must have all
    necessary information, including a name and description, an organizer, at least one ticket, and valid payment options.
    This API endpoint will return argument errors for event fields that fail to validate the publish requirements. Returns
    a boolean indicating success or failure of the publish.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublish-post-openapi.md
- name: Eventbrite - Post Events Unpublish
  x-api-slug: eventsidunpublish-post
  description: |-
    Unpublishes an event. In order for a free event to be unpublished, it must not have any pending or completed orders,
    even if the event is in the past. In order for a paid event to be unpublished, it must not have any pending or completed
    orders, unless the event has been completed and paid out. Returns a boolean indicating success or failure of the
    unpublish.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidunpublish-post-openapi.md
- name: Eventbrite - Post Events Cancel
  x-api-slug: eventsidcancel-post
  description: |-
    Cancels an event if it has not already been deleted. In order for cancel to be permitted, there must be no pending or
    completed orders. Returns a boolean indicating success or failure of the cancel.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidcancel-post-openapi.md
- name: Eventbrite - Post Events Copy
  x-api-slug: eventsidcopy-post
  description: Creates a duplicate version of the event being copied. Returns the
    event object for the newly created event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidcopy-post-openapi.md
- name: Eventbrite - Delete Events
  x-api-slug: eventsid-delete
  description: |-
    Deletes an event if the delete is permitted. In order for a delete to be permitted, there must be no pending or
    completed orders. Returns a boolean indicating success or failure of the delete.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsid-delete-openapi.md
- name: Eventbrite - Get Events Display Settings
  x-api-slug: eventsiddisplay-settings-get
  description: Retrieves the display settings for an event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddisplay-settings-get-openapi.md
- name: Eventbrite - Post Events Display Settings
  x-api-slug: eventsiddisplay-settings-post
  description: Updates the display settings for an event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddisplay-settings-post-openapi.md
- name: Eventbrite - Get Events Ticket Classes
  x-api-slug: eventsidticket-classes-get
  description: |-
    Returns a paginated response with a key of
    ticket_classes, containing a list of ticket_class.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classes-get-openapi.md
- name: Eventbrite - Post Events Ticket Classes
  x-api-slug: eventsidticket-classes-post
  description: |-
    Creates a new ticket class, returning the result as a ticket_class
    under the key ticket_class.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classes-post-openapi.md
- name: Eventbrite - Get Events Ticket Classes Ticket Class
  x-api-slug: eventsidticket-classesticket-class-id-get
  description: |-
    Gets and returns a single ticket_class by ID, as the key
    ticket_class.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classesticket-class-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classesticket-class-id-get-openapi.md
- name: Eventbrite - Post Events Ticket Classes Ticket Class
  x-api-slug: eventsidticket-classesticket-class-id-post
  description: Updates an existing ticket class, returning the updated result as a
    ticket_class under the key ticket_class.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classesticket-class-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classesticket-class-id-post-openapi.md
- name: Eventbrite - Delete Events Ticket Classes Ticket Class
  x-api-slug: eventsidticket-classesticket-class-id-delete
  description: 'Deletes the ticket class. Returns {&quot;deleted&quot;: true}.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classesticket-class-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-classesticket-class-id-delete-openapi.md
- name: Eventbrite - Get Events Canned Questions
  x-api-slug: eventsidcanned-questions-get
  description: 'This endpoint returns canned questions of a single event (examples:
    first name, last name, company, prefix, etc.). This endpoint will return question.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidcanned-questions-get-openapi.md
- name: Eventbrite - Post Events Canned Questions
  x-api-slug: eventsidcanned-questions-post
  description: Creates a new canned question; returns the result as a question.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidcanned-questions-post-openapi.md
- name: Eventbrite - Get Events Questions
  x-api-slug: eventsidquestions-get
  description: |-
    Eventbrite allows event organizers to add custom questions that attendees fill
    out upon registration. This endpoint can be helpful for determining what
    custom information is collected and available per event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidquestions-get-openapi.md
- name: Eventbrite - Post Events Questions
  x-api-slug: eventsidquestions-post
  description: Creates a new question; returns the result as a question as the key
    question.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidquestions-post-openapi.md
- name: Eventbrite - Get Events Questions
  x-api-slug: eventsidquestionsid-get
  description: This endpoint will return question for a specific question id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidquestionsid-get-openapi.md
- name: Eventbrite - Get Events Attendees Attendee
  x-api-slug: eventsidattendeesattendee-id-get
  description: Returns a single attendee by ID, as the key attendee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidattendeesattendee-id-get-openapi.md
- name: Eventbrite - Get Events Orders
  x-api-slug: eventsidorders-get
  description: Returns a paginated response with a key of orders, containing a list
    of order against this event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidorders-get-openapi.md
- name: Eventbrite - Get Events Discounts
  x-api-slug: eventsiddiscounts-get
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscounts-get-openapi.md
- name: Eventbrite - Post Events Discounts
  x-api-slug: eventsiddiscounts-post
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscounts-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscounts-post-openapi.md
- name: Eventbrite - Get Events Discounts Discount
  x-api-slug: eventsiddiscountsdiscount-id-get
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscountsdiscount-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscountsdiscount-id-get-openapi.md
- name: Eventbrite - Post Events Discounts Discount
  x-api-slug: eventsiddiscountsdiscount-id-post
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscountsdiscount-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscountsdiscount-id-post-openapi.md
- name: Eventbrite - Delete Events Discounts Discount
  x-api-slug: eventsiddiscountsdiscount-id-delete
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscountsdiscount-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsiddiscountsdiscount-id-delete-openapi.md
- name: Eventbrite - Get Events Public Discounts
  x-api-slug: eventsidpublic-discounts-get
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discounts-get-openapi.md
- name: Eventbrite - Post Events Public Discounts
  x-api-slug: eventsidpublic-discounts-post
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discounts-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discounts-post-openapi.md
- name: Eventbrite - Get Events Public Discounts Discount
  x-api-slug: eventsidpublic-discountsdiscount-id-get
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discountsdiscount-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discountsdiscount-id-get-openapi.md
- name: Eventbrite - Post Events Public Discounts Discount
  x-api-slug: eventsidpublic-discountsdiscount-id-post
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discountsdiscount-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discountsdiscount-id-post-openapi.md
- name: Eventbrite - Delete Events Public Discounts Discount
  x-api-slug: eventsidpublic-discountsdiscount-id-delete
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discountsdiscount-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidpublic-discountsdiscount-id-delete-openapi.md
- name: Eventbrite - Get Events Access Codes
  x-api-slug: eventsidaccess-codes-get
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidaccess-codes-get-openapi.md
- name: Eventbrite - Post Events Access Codes
  x-api-slug: eventsidaccess-codes-post
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidaccess-codes-post-openapi.md
- name: Eventbrite - Get Events Access Codes Access Code
  x-api-slug: eventsidaccess-codesaccess-code-id-get
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidaccess-codesaccess-code-id-get-openapi.md
- name: Eventbrite - Post Events Access Codes Access Code
  x-api-slug: eventsidaccess-codesaccess-code-id-post
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidaccess-codesaccess-code-id-post-openapi.md
- name: Eventbrite - Delete Events Access Codes
  x-api-slug: eventsidaccess-codes-delete
  description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidaccess-codes-delete-openapi.md
- name: Eventbrite - Get Events Transfers
  x-api-slug: eventsidtransfers-get
  description: Returns a list of transfers for the event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidtransfers-get-openapi.md
- name: Eventbrite - Get Events Teams
  x-api-slug: eventsidteams-get
  description: Returns a list of attendee-team for the event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidteams-get-openapi.md
- name: Eventbrite - Get Events Teams
  x-api-slug: eventsidteamsid-get
  description: Returns information for a single attendee-team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidteamsid-get-openapi.md
- name: Eventbrite - Get Events Teams Attendees
  x-api-slug: eventsidteamsidattendees-get
  description: Returns attendee for a single attendee-team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidteamsidattendees-get-openapi.md
- name: Eventbrite - Get Events Event Ticket Groups
  x-api-slug: eventsevent-idticket-groups-get
  description: |-
    Get the list of ticket_group for the event with the specified :event_id.
    By default, only the ticket groups that are live are shown.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-groups-get-openapi.md
- name: Eventbrite - Post Events Event Ticket Classes Ticket Class Ticket Groups Ticket
    Group
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post
  description: Add the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id to the Ticket Group identified by :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post-openapi.md
- name: Eventbrite - Delete Events Event Ticket Classes Ticket Class Ticket Groups
    Ticket Group
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete
  description: Remove the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id from the Ticket Group identified by :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete-openapi.md
- name: Eventbrite - Get Events Event Ticket Classes Ticket Class Ticket Groups
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groups-get
  description: |-
    Get the Ticket Groups for Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id.
    By default, only the ticket groups that are live are shown.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groups-get-openapi.md
- name: Eventbrite - Get Events Ticket Buyer Settings
  x-api-slug: eventsidticket-buyer-settings-get
  description: Returns a ticket_buyer_settings for an event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-buyer-settings-get-openapi.md
- name: Eventbrite - Post Events Ticket Buyer Settings
  x-api-slug: eventsidticket-buyer-settings-post
  description: Updates the ticket buyer settings for an event. Returns a ticket_buyer_settings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsidticket-buyer-settings-post-openapi.md
- name: Eventbrite - Get Organizers Events
  x-api-slug: organizersidevents-get
  description: Gets events of the organizer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/organizersidevents-get-openapi.md
- name: Eventbrite - Get Events Event Tracking Beacons
  x-api-slug: eventsevent-idtracking-beacons-get
  description: Returns the list of tracking_beacon for the event :event_id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idtracking-beacons-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idtracking-beacons-get-openapi.md
- name: Eventbrite - Get Users Owned Events
  x-api-slug: usersidowned-events-get
  description: |-
    Returns a paginated response of events, under
    the key events, of all events the user owns (i.e. events they are organising)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersidowned-events-get-openapi.md
- name: Eventbrite - Get Users Events
  x-api-slug: usersidevents-get
  description: Returns a paginated response of events, under the key events, of all
    events the user has access to
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersidevents-get-openapi.md
- name: Eventbrite - Post Organizations Events
  x-api-slug: organizationsidevents-post
  description: Creates new events objects under an organization and returns it as
    event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/organizationsidevents-post-openapi.md
- name: Eventbrite - Post Users User Events Event Ticket Classes Ticket Class Ticket
    Groups
  x-api-slug: usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post
  description: |-
    Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that
    belongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.
    If the list provided is empty, remove this ticket class from every ticket group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-openapi.md
- name: Eventbrite - Get Venues Events
  x-api-slug: venuesidevents-get
  description: Returns events of a given venue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/venuesidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/venuesidevents-get-openapi.md
- name: Eventbrite - Get Series Events
  x-api-slug: seriesidevents-get
  description: Returns all of the events that belong to this repeating event series.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/seriesidevents-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/seriesidevents-get-openapi.md
- name: Eventbrite - Post Series Events
  x-api-slug: seriesidevents-post
  description: |-
    Creates more event dates or updates or deletes existing event dates in a repeating event series. In order for a series
    date to be deleted or updated, there must be no pending or completed orders for that date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/seriesidevents-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/seriesidevents-post-openapi.md
- name: Eventbrite - Get User List Events
  x-api-slug: user-list-events-get
  description: This method lists the events created by this user. Only public events
    are returned if no authentication is passed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/user-list-events-get-openapi.md
- name: Eventbrite - Get Organizer List Events
  x-api-slug: organizer-list-events-get
  description: This method returns a list of events for a given organizer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/organizer-list-events-get-openapi.md
- name: Eventbrite - Get Users Owned Event Attendees
  x-api-slug: usersidowned-event-attendees-get
  description: |-
    Returns a paginated response of attendees,
    under the key attendees, of attendees visiting any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersidowned-event-attendees-get-openapi.md
- name: Eventbrite - Get Users Owned Event Orders
  x-api-slug: usersidowned-event-orders-get
  description: |-
    Returns a paginated response of orders,
    under the key orders, of orders placed against any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersidowned-event-orders-get-openapi.md
- name: Eventbrite - Get Event Search
  x-api-slug: event-search-get
  description: This method uses our search index to find publicly listed events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-search-get-openapi.md
- name: Eventbrite - Get Event Get
  x-api-slug: event-get-get
  description: This method returns the data for a given event. Only public events
    are viewable if no authentication is passed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-get-get-openapi.md
- name: Eventbrite - Get Event New
  x-api-slug: event-new-get
  description: This method creates a new event. It returns the ID of the newly created
    event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-new-get-openapi.md
- name: Eventbrite - Get Event Update
  x-api-slug: event-update-get
  description: This method updates an existing event. Only the fields passed as arguments
    will be modified. This method returns the ID of the modified event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-update-get-openapi.md
- name: Eventbrite - Get Event Copy
  x-api-slug: event-copy-get
  description: This method duplicates an existing event, returning the ID of the new
    event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-copy-get-openapi.md
- name: Eventbrite - Get Event List Attendees
  x-api-slug: event-list-attendees-get
  description: This method returns a list of attendees for a given event. If no authentication
    is passed, only publicly available attendee records will be returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-attendees-get-openapi.md
- name: Eventbrite - Get Event List Discounts
  x-api-slug: event-list-discounts-get
  description: This method returns a list of discounts for a given event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-discounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-discounts-get-openapi.md
- name: Eventbrite - Get Events Event Checkout Settings
  x-api-slug: eventsevent-idcheckout-settings-get
  description: Gets and returns a list of checkout_settings associated with a given
    event by its event_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idcheckout-settings-get-openapi.md
- name: Eventbrite - Post Events Event Checkout Settings
  x-api-slug: eventsevent-idcheckout-settings-post
  description: Associate a single or set of checkout_settings with a given event by
    its event_id. This does not add more checkout settings to the event, but instead
    replaces all checkout settings for the event with the one(s) submitted. The JSON
    post body is a string list of the checkout_settings IDs you want to associate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idcheckout-settings-post-openapi.md
- name: Eventbrite - Get Events Event Payout Settings
  x-api-slug: eventsevent-idpayout-settings-get
  description: Gets and returns the payout_settings (user instrument ID) associated
    with a given event by its event_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idpayout-settings-get-openapi.md
- name: Eventbrite - Post Events Event Payout Settings
  x-api-slug: eventsevent-idpayout-settings-post
  description: Associate a payout user instrument ID with a given event, or clear
    the association by passing a null value for the user instrument ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idpayout-settings-post-openapi.md
- name: Eventbrite - Get Events Event Ticket Groups
  x-api-slug: eventsevent-idticket-groups-get
  description: |-
    Get the list of ticket_group for the event with the specified :event_id.
    By default, only the ticket groups that are live are shown.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-groups-get-openapi.md
- name: Eventbrite - Post Events Event Ticket Classes Ticket Class Ticket Groups Ticket
    Group
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post
  description: Add the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id to the Ticket Group identified by :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post-openapi.md
- name: Eventbrite - Delete Events Event Ticket Classes Ticket Class Ticket Groups
    Ticket Group
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete
  description: Remove the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id from the Ticket Group identified by :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete-openapi.md
- name: Eventbrite - Get Events Event Ticket Classes Ticket Class Ticket Groups
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groups-get
  description: |-
    Get the Ticket Groups for Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id.
    By default, only the ticket groups that are live are shown.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groups-get-openapi.md
- name: Eventbrite - Get Events Event Tracking Beacons
  x-api-slug: eventsevent-idtracking-beacons-get
  description: Returns the list of tracking_beacon for the event :event_id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idtracking-beacons-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idtracking-beacons-get-openapi.md
- name: Eventbrite - Get Users Owned Event Attendees
  x-api-slug: usersidowned-event-attendees-get
  description: |-
    Returns a paginated response of attendees,
    under the key attendees, of attendees visiting any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersidowned-event-attendees-get-openapi.md
- name: Eventbrite - Get Users Owned Event Orders
  x-api-slug: usersidowned-event-orders-get
  description: |-
    Returns a paginated response of orders,
    under the key orders, of orders placed against any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersidowned-event-orders-get-openapi.md
- name: Eventbrite - Post Users User Events Event Ticket Classes Ticket Class Ticket
    Groups
  x-api-slug: usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post
  description: |-
    Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that
    belongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.
    If the list provided is empty, remove this ticket class from every ticket group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-openapi.md
- name: Eventbrite - Get Event Search
  x-api-slug: event-search-get
  description: This method uses our search index to find publicly listed events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-search-get-openapi.md
- name: Eventbrite - Get Event Get
  x-api-slug: event-get-get
  description: This method returns the data for a given event. Only public events
    are viewable if no authentication is passed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-get-get-openapi.md
- name: Eventbrite - Get Event New
  x-api-slug: event-new-get
  description: This method creates a new event. It returns the ID of the newly created
    event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-new-get-openapi.md
- name: Eventbrite - Get Event Update
  x-api-slug: event-update-get
  description: This method updates an existing event. Only the fields passed as arguments
    will be modified. This method returns the ID of the modified event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-update-get-openapi.md
- name: Eventbrite - Get Event Copy
  x-api-slug: event-copy-get
  description: This method duplicates an existing event, returning the ID of the new
    event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-copy-get-openapi.md
- name: Eventbrite - Get Event List Attendees
  x-api-slug: event-list-attendees-get
  description: This method returns a list of attendees for a given event. If no authentication
    is passed, only publicly available attendee records will be returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-attendees-get-openapi.md
- name: Eventbrite - Get Event List Discounts
  x-api-slug: event-list-discounts-get
  description: This method returns a list of discounts for a given event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-discounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-discounts-get-openapi.md
- name: Eventbrite - Get Event List Discounts
  x-api-slug: event-list-discounts-get
  description: This method returns a list of discounts for a given event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-discounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-discounts-get-openapi.md
- name: Eventbrite - Get Event List Attendees
  x-api-slug: event-list-attendees-get
  description: This method returns a list of attendees for a given event. If no authentication
    is passed, only publicly available attendee records will be returned.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-list-attendees-get-openapi.md
- name: Eventbrite - Get Event Copy
  x-api-slug: event-copy-get
  description: This method duplicates an existing event, returning the ID of the new
    event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-copy-get-openapi.md
- name: Eventbrite - Get Event Update
  x-api-slug: event-update-get
  description: This method updates an existing event. Only the fields passed as arguments
    will be modified. This method returns the ID of the modified event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-update-get-openapi.md
- name: Eventbrite - Get Event New
  x-api-slug: event-new-get
  description: This method creates a new event. It returns the ID of the newly created
    event.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-new-get-openapi.md
- name: Eventbrite - Get Event Get
  x-api-slug: event-get-get
  description: This method returns the data for a given event. Only public events
    are viewable if no authentication is passed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-get-get-openapi.md
- name: Eventbrite - Get Event Search
  x-api-slug: event-search-get
  description: This method uses our search index to find publicly listed events.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/event-search-get-openapi.md
- name: Eventbrite - Post Users User Events Event Ticket Classes Ticket Class Ticket
    Groups
  x-api-slug: usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post
  description: |-
    Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that
    belongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.
    If the list provided is empty, remove this ticket class from every ticket group.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post-openapi.md
- name: Eventbrite - Get Users Owned Event Orders
  x-api-slug: usersidowned-event-orders-get
  description: |-
    Returns a paginated response of orders,
    under the key orders, of orders placed against any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersidowned-event-orders-get-openapi.md
- name: Eventbrite - Get Users Owned Event Attendees
  x-api-slug: usersidowned-event-attendees-get
  description: |-
    Returns a paginated response of attendees,
    under the key attendees, of attendees visiting any of the events the user owns
    (events that would be returned from /users/:id/owned_events/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/usersidowned-event-attendees-get-openapi.md
- name: Eventbrite - Get Events Event Tracking Beacons
  x-api-slug: eventsevent-idtracking-beacons-get
  description: Returns the list of tracking_beacon for the event :event_id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idtracking-beacons-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idtracking-beacons-get-openapi.md
- name: Eventbrite - Get Events Event Ticket Classes Ticket Class Ticket Groups
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groups-get
  description: |-
    Get the Ticket Groups for Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id.
    By default, only the ticket groups that are live are shown.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groups-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groups-get-openapi.md
- name: Eventbrite - Delete Events Event Ticket Classes Ticket Class Ticket Groups
    Ticket Group
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete
  description: Remove the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id from the Ticket Group identified by :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete-openapi.md
- name: Eventbrite - Post Events Event Ticket Classes Ticket Class Ticket Groups Ticket
    Group
  x-api-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post
  description: Add the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id to the Ticket Group identified by :ticket_group_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post-openapi.md
- name: Eventbrite - Get Events Event Ticket Groups
  x-api-slug: eventsevent-idticket-groups-get
  description: |-
    Get the list of ticket_group for the event with the specified :event_id.
    By default, only the ticket groups that are live are shown.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idticket-groups-get-openapi.md
- name: Eventbrite - Post Events Event Payout Settings
  x-api-slug: eventsevent-idpayout-settings-post
  description: Associate a payout user instrument ID with a given event, or clear
    the association by passing a null value for the user instrument ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idpayout-settings-post-openapi.md
- name: Eventbrite - Get Events Event Payout Settings
  x-api-slug: eventsevent-idpayout-settings-get
  description: Gets and returns the payout_settings (user instrument ID) associated
    with a given event by its event_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idpayout-settings-get-openapi.md
- name: Eventbrite - Post Events Event Checkout Settings
  x-api-slug: eventsevent-idcheckout-settings-post
  description: Associate a single or set of checkout_settings with a given event by
    its event_id. This does not add more checkout settings to the event, but instead
    replaces all checkout settings for the event with the one(s) submitted. The JSON
    post body is a string list of the checkout_settings IDs you want to associate.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idcheckout-settings-post-openapi.md
- name: Eventbrite - Get Events Event Checkout Settings
  x-api-slug: eventsevent-idcheckout-settings-get
  description: Gets and returns a list of checkout_settings associated with a given
    event by its event_id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Events, Tickets, Events, My API Stack, API LIfeyclessss, Stack Network, Stack,
    Marketplace, Technology, Mobile, internet, API Provider, Tickets, Profiles, Registrations,
    General Data, Relative Data, Pedestal, Historical Data API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/eventbrite/eventsevent-idcheckout-settings-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://europeana.api.gallery.streamdata.io
- type: x-api-stack
  url: http://eventbrite.stack.network
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/eventbrite/apidescription?format=internal&ver=1351170233000
- type: x-authentication
  url: https://developer.eventbrite.com/docs/auth/
- type: x-base
  url: https://www.eventbriteapi.com/
- type: x-blog
  url: http://blog.eventbrite.com/
- type: x-blog-rss
  url: http://blog.eventbrite.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/eventbrite
- type: x-crunchbase
  url: https://crunchbase.com/organization/eventbrite
- type: x-developer
  url: https://developer.eventbrite.com/
- type: x-github
  url: https://github.com/eventbrite
- type: x-pricing
  url: http://help.eventbrite.com/customer/en_us/portal/articles/428604
- type: x-privacy
  url: http://www.eventbrite.com/privacypolicy
- type: x-sdks-io
  url: https://sdks.io/SDK/View/eventbrite
- type: x-selfservice-registration
  url: https://www.eventbrite.com/signup/?referrer=%2F%3Fshow_onboarding%3D1&user_type=prebuyer&user_type_sig=AH_ElWGNJ_zHaAxwjzt5jiCRmvPvNBsy6w
- type: x-terms-of-service
  url: http://www.eventbrite.com/tos
- type: x-twitter
  url: https://twitter.com/EventbriteAPI
- type: x-twitter
  url: https://twitter.com/eventbrite
- type: x-website
  url: http://eventbriteapi.com
- type: x-website
  url: http://developer.eventbrite.com/
- type: x-website
  url: http://eventbrite.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---