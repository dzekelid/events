---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Delete Events Event Ticket Classes Ticket Class Ticket Groups
    Ticket Group
  description: Remove the Ticket Class with the specified :ticket_class_id that belongs
    to the event with :event_id from the Ticket Group identified by :ticket_group_id.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/:
    post:
      summary: Post Events
      description: Makes a new event, and returns an event for the specified event.
      operationId: postEvents
      x-api-path-slug: events-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: event.capacity
        description: Set specific capacity (if omitted, sums ticket capacities)
        type: query
      - in: query
        name: event.category_id
        description: The category (vertical) of the event
        type: query
      - in: query
        name: event.currency
        description: Event currency (3 letter code)
        type: query
      - in: query
        name: event.description.html
        description: The description on the event page
        type: query
      - in: query
        name: event.end.timezone
        description: End time timezone (Olson format)
        type: query
      - in: query
        name: event.end.utc
        description: The end time of the event
        type: query
      - in: query
        name: event.format_id
        description: The format (general type) of the event
        type: query
      - in: query
        name: event.hide_end_date
        description: Whether the end date should be hidden
        type: query
      - in: query
        name: event.hide_start_date
        description: Whether the start date should be hidden
        type: query
      - in: query
        name: event.invite_only
        description: Only invited users can see the event page
        type: query
      - in: query
        name: event.is_reserved_seating
        description: If the event is reserved seating
        type: query
      - in: query
        name: event.listed
        description: If the event is publicly listed and searchable
        type: query
      - in: query
        name: event.logo.id
        description: (Deprecated) The logo for the event
        type: query
      - in: query
        name: event.logo_id
        description: The logo for the event
        type: query
      - in: query
        name: event.name.html
        description: The name of the event
        type: query
      - in: query
        name: event.online_event
        description: Is the event online-only (no venue)?
        type: query
      - in: query
        name: event.organizer_id
        description: The ID of the organizer of this event
        type: query
      - in: query
        name: event.password
        description: Password needed to see the event in unlisted mode
        type: query
      - in: query
        name: event.shareable
        description: If users can share the event on social media
        type: query
      - in: query
        name: event.show_pick_a_seat
        description: For reserved seating event, if attendees can pick their seats
        type: query
      - in: query
        name: event.show_remaining
        description: If the remaining number of tickets is publicly visible on the
          event page
        type: query
      - in: query
        name: event.show_seatmap_thumbnail
        description: For reserved seating event, if venue map thumbnail visible on
          the event page
        type: query
      - in: query
        name: event.source
        description: Source of the event (defaults to API)
        type: query
      - in: query
        name: event.start.timezone
        description: Start time timezone (Olson format)
        type: query
      - in: query
        name: event.start.utc
        description: The start time of the event
        type: query
      - in: query
        name: event.subcategory_id
        description: The subcategory of the event (US only)
        type: query
      - in: query
        name: event.venue_id
        description: The ID of a previously-created venue to associate with this event
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}:
    get:
      summary: Get Events
      description: Returns an event for the specified event. Many of Eventbrite?s
        API use cases resolve around pulling details of a specific event within an
        Eventbrite account.
      operationId: getEvents
      x-api-path-slug: eventsid-get
      parameters:
      - in: path
        name: id
        description: Event Id
      responses:
        200:
          description: OK
      tags:
      - Events
    post:
      summary: Post Events
      description: Updates an event. Returns an event for the specified event.
      operationId: postEvents
      x-api-path-slug: eventsid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Event Id
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/:event_id/checkout_settings/:
    get:
      summary: Get Events Event Checkout Settings
      description: Gets and returns a list of checkout_settings associated with a
        given event by its event_id.
      operationId: getEventsEventCheckoutSettings
      x-api-path-slug: eventsevent-idcheckout-settings-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Checkout
      - Settings
    post:
      summary: Post Events Event Checkout Settings
      description: Associate a single or set of checkout_settings with a given event
        by its event_id. This does not add more checkout settings to the event, but
        instead replaces all checkout settings for the event with the one(s) submitted.
        The JSON post body is a string list of the checkout_settings IDs you want
        to associate.
      operationId: postEventsEventCheckoutSettings
      x-api-path-slug: eventsevent-idcheckout-settings-post
      parameters:
      - in: query
        name: checkout_settings_ids
        description: A list of IDs for checkout settings that should be linked to
          the event
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Checkout
      - Settings
  /events/:event_id/payout_settings/:
    get:
      summary: Get Events Event Payout Settings
      description: Gets and returns the payout_settings (user instrument ID) associated
        with a given event by its event_id.
      operationId: getEventsEventPayoutSettings
      x-api-path-slug: eventsevent-idpayout-settings-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Payout
      - Settings
    post:
      summary: Post Events Event Payout Settings
      description: Associate a payout user instrument ID with a given event, or clear
        the association by passing a null value for the user instrument ID.
      operationId: postEventsEventPayoutSettings
      x-api-path-slug: eventsevent-idpayout-settings-post
      parameters:
      - in: query
        name: payout_settings.user_instrument_vault_id
        description: The vault ID for the user instrument to which payouts are sent
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Payout
      - Settings
  /events/{id}/:
    get:
      summary: Get Events
      description: |-
        Returns an event for the specified event. Many of Eventbrite???s API use cases revolve around pulling details
        of a specific event within an Eventbrite account. Does not support fetching a repeating event series parent
        (see GET /series/:id/).
      operationId: getEvents
      x-api-path-slug: eventsid-get
      responses:
        200:
          description: OK
      tags:
      - Events
    post:
      summary: Post Events
      description: |-
        Updates an event. Returns an event for the specified event. Does not support updating a repeating event
        series parent (see POST /series/:id/).
      operationId: postEvents
      x-api-path-slug: eventsid-post
      parameters:
      - in: query
        name: event.capacity
        description: Set specific capacity (if omitted, sums ticket capacities)
        type: query
      - in: query
        name: event.category_id
        description: The category (vertical) of the event
        type: query
      - in: query
        name: event.currency
        description: Event currency (3 letter code)
        type: query
      - in: query
        name: event.description.html
        description: The description on the event page
        type: query
      - in: query
        name: event.end.timezone
        description: End time timezone (Olson format)
        type: query
      - in: query
        name: event.end.utc
        description: The end time of the event
        type: query
      - in: query
        name: event.format_id
        description: The format (general type) of the event
        type: query
      - in: query
        name: event.hide_end_date
        description: Whether the end date should be hidden
        type: query
      - in: query
        name: event.hide_start_date
        description: Whether the start date should be hidden
        type: query
      - in: query
        name: event.invite_only
        description: Only invited users can see the event page
        type: query
      - in: query
        name: event.is_reserved_seating
        description: If the event is reserved seating
        type: query
      - in: query
        name: event.listed
        description: If the event is publicly listed and searchable
        type: query
      - in: query
        name: event.logo.id
        description: (Deprecated) The logo for the event
        type: query
      - in: query
        name: event.logo_id
        description: The logo for the event
        type: query
      - in: query
        name: event.name.html
        description: The name of the event
        type: query
      - in: query
        name: event.online_event
        description: Is the event online-only (no venue)?
        type: query
      - in: query
        name: event.organizer_id
        description: The ID of the organizer of this event
        type: query
      - in: query
        name: event.password
        description: Password needed to see the event in unlisted mode
        type: query
      - in: query
        name: event.shareable
        description: If users can share the event on social media
        type: query
      - in: query
        name: event.show_pick_a_seat
        description: For reserved seating event, if attendees can pick their seats
        type: query
      - in: query
        name: event.show_remaining
        description: If the remaining number of tickets is publicly visible on the
          event page
        type: query
      - in: query
        name: event.show_seatmap_thumbnail
        description: For reserved seating event, if venue map thumbnail visible on
          the event page
        type: query
      - in: query
        name: event.source
        description: Source of the event (defaults to API)
        type: query
      - in: query
        name: event.start.timezone
        description: Start time timezone (Olson format)
        type: query
      - in: query
        name: event.start.utc
        description: The start time of the event
        type: query
      - in: query
        name: event.subcategory_id
        description: The subcategory of the event (US only)
        type: query
      - in: query
        name: event.venue_id
        description: ID of the venue
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
    delete:
      summary: Delete Events
      description: |-
        Deletes an event if the delete is permitted. In order for a delete to be permitted, there must be no pending or
        completed orders. Returns a boolean indicating success or failure of the delete.
      operationId: deleteEvents
      x-api-path-slug: eventsid-delete
      responses:
        200:
          description: OK
      tags:
      - Events
  /events/{id}/publish/:
    post:
      summary: Post Events Publish
      description: |-
        Publishes an event if it has not already been deleted. In order for publish to be permitted, the event must have all
        necessary information, including a name and description, an organizer, at least one ticket, and valid payment options.
        This API endpoint will return argument errors for event fields that fail to validate the publish requirements. Returns
        a boolean indicating success or failure of the publish.
      operationId: postEventsPublish
      x-api-path-slug: eventsidpublish-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Publish
  /events/{id}/unpublish/:
    post:
      summary: Post Events Unpublish
      description: |-
        Unpublishes an event. In order for a free event to be unpublished, it must not have any pending or completed orders,
        even if the event is in the past. In order for a paid event to be unpublished, it must not have any pending or completed
        orders, unless the event has been completed and paid out. Returns a boolean indicating success or failure of the
        unpublish.
      operationId: postEventsUnpublish
      x-api-path-slug: eventsidunpublish-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Unpublish
  /events/{id}/cancel/:
    post:
      summary: Post Events Cancel
      description: |-
        Cancels an event if it has not already been deleted. In order for cancel to be permitted, there must be no pending or
        completed orders. Returns a boolean indicating success or failure of the cancel.
      operationId: postEventsCancel
      x-api-path-slug: eventsidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Cancel
  /events/{id}/copy/:
    post:
      summary: Post Events Copy
      description: Creates a duplicate version of the event being copied. Returns
        the event object for the newly created event.
      operationId: postEventsCopy
      x-api-path-slug: eventsidcopy-post
      parameters:
      - in: query
        name: end_date
        description: The end time of the new event
        type: query
      - in: query
        name: name
        description: The name of the new event
        type: query
      - in: query
        name: start_date
        description: The start time of the new event
        type: query
      - in: query
        name: timezone
        description: timezone for the new event (Olson format)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Copy
  /events/{id}/display_settings/:
    get:
      summary: Get Events Display Settings
      description: Retrieves the display settings for an event.
      operationId: getEventsDisplaySettings
      x-api-path-slug: eventsiddisplay-settings-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Display
      - Settings
    post:
      summary: Post Events Display Settings
      description: Updates the display settings for an event.
      operationId: postEventsDisplaySettings
      x-api-path-slug: eventsiddisplay-settings-post
      parameters:
      - in: query
        name: display_settings.show_end_date
        description: Whether to display the end date on the event listing
        type: query
      - in: query
        name: display_settings.show_facebook_friends_going
        description: Whether to display which of the user&#8217;s Facebook friends
          are going
        type: query
      - in: query
        name: display_settings.show_map
        description: Whether to display a map to the venue on the event listing
        type: query
      - in: query
        name: display_settings.show_organizer_facebook
        description: Whether to display a link to the organizer&#8217;s Facebook profile
        type: query
      - in: query
        name: display_settings.show_organizer_twitter
        description: Whether to display a link to the organizer&#8217;s Twitter profile
        type: query
      - in: query
        name: display_settings.show_remaining
        description: Whether to display the number of remaining tickets
        type: query
      - in: query
        name: display_settings.show_start_date
        description: Whether to display the start date on the event listing
        type: query
      - in: query
        name: display_settings.show_start_end_time
        description: Whether to display event start and end time on the event listing
        type: query
      - in: query
        name: display_settings.show_timezone
        description: Whether to display the event timezone on the event listing
        type: query
      - in: query
        name: display_settings.terminology
        description: 'Which terminology should be used to refer to the event (Valid
          choices are: tickets_vertical, or endurance_vertical)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Display
      - Settings
  /events/{id}/ticket_classes/:
    get:
      summary: Get Events Ticket Classes
      description: |-
        Returns a paginated response with a key of
        ticket_classes, containing a list of ticket_class.
      operationId: getEventsTicketClasses
      x-api-path-slug: eventsidticket-classes-get
      parameters:
      - in: query
        name: pos
        description: 'Only return ticket classes valid for the given point of sale
          (Valid choices are: online, or at_the_door)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
    post:
      summary: Post Events Ticket Classes
      description: |-
        Creates a new ticket class, returning the result as a ticket_class
        under the key ticket_class.
      operationId: postEventsTicketClasses
      x-api-path-slug: eventsidticket-classes-post
      parameters:
      - in: query
        name: ticket_class.auto_hide
        description: Hide this ticket when it is not on sale
        type: query
      - in: query
        name: ticket_class.auto_hide_after
        description: Override re-hide date for auto-hide
        type: query
      - in: query
        name: ticket_class.auto_hide_before
        description: Override reveal date for auto-hide
        type: query
      - in: query
        name: ticket_class.cost
        description: Cost of the ticket (currently currency must match event currency)
          e
        type: query
      - in: query
        name: ticket_class.description
        description: Description of the ticket
        type: query
      - in: query
        name: ticket_class.donation
        description: Is this a donation? (user-supplied cost)
        type: query
      - in: query
        name: ticket_class.free
        description: Is this a free ticket?
        type: query
      - in: query
        name: ticket_class.hidden
        description: Hide this ticket
        type: query
      - in: query
        name: ticket_class.hide_description
        description: Hide the ticket description on the event page
        type: query
      - in: query
        name: ticket_class.include_fee
        description: Absorb the fee into the displayed cost
        type: query
      - in: query
        name: ticket_class.maximum_quantity
        description: Maximum number per order (blank for unlimited)
        type: query
      - in: query
        name: ticket_class.minimum_quantity
        description: Minimum number per order
        type: query
      - in: query
        name: ticket_class.name
        description: Name of this ticket type
        type: query
      - in: query
        name: ticket_class.order_confirmation_message
        description: Order message per ticket type
        type: query
      - in: query
        name: ticket_class.quantity_total
        description: Total available number of this ticket, required for non-donation
          tickets
        type: query
      - in: query
        name: ticket_class.sales_channels
        description: A list of all supported sales channels ([&#8220;online&#8221;],
          [&#8220;online&#8221;, &#8220;atd&#8221;], [&#8220;atd&#8221;])
        type: query
      - in: query
        name: ticket_class.sales_end
        description: When the ticket stops being on sale (leave empty for &#8216;one
          hour before event start&#8217;)
        type: query
      - in: query
        name: ticket_class.sales_start
        description: When the ticket is available for sale (leave empty for &#8216;when
          event published&#8217;)
        type: query
      - in: query
        name: ticket_class.sales_start_after
        description: The ID of another ticket class - when it sells out, this class
          will go on sale
        type: query
      - in: query
        name: ticket_class.split_fee
        description: Absorb the payment fee, but show the eventbrite fee
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
  /events/{id}/ticket_classes/:ticket_class_id/:
    get:
      summary: Get Events Ticket Classes Ticket Class
      description: |-
        Gets and returns a single ticket_class by ID, as the key
        ticket_class.
      operationId: getEventsTicketClassesTicketClass
      x-api-path-slug: eventsidticket-classesticket-class-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
      - :ticket
      - Class
    post:
      summary: Post Events Ticket Classes Ticket Class
      description: Updates an existing ticket class, returning the updated result
        as a ticket_class under the key ticket_class.
      operationId: postEventsTicketClassesTicketClass
      x-api-path-slug: eventsidticket-classesticket-class-id-post
      parameters:
      - in: query
        name: ticket_class.auto_hide
        description: Hide this ticket when it is not on sale
        type: query
      - in: query
        name: ticket_class.auto_hide_after
        description: Override re-hide date for auto-hide
        type: query
      - in: query
        name: ticket_class.auto_hide_before
        description: Override reveal date for auto-hide
        type: query
      - in: query
        name: ticket_class.cost
        description: Cost of the ticket (currently currency must match event currency)
          e
        type: query
      - in: query
        name: ticket_class.description
        description: Description of the ticket
        type: query
      - in: query
        name: ticket_class.donation
        description: Is this a donation? (user-supplied cost)
        type: query
      - in: query
        name: ticket_class.free
        description: Is this a free ticket?
        type: query
      - in: query
        name: ticket_class.hidden
        description: Hide this ticket
        type: query
      - in: query
        name: ticket_class.hide_description
        description: Hide the ticket description on the event page
        type: query
      - in: query
        name: ticket_class.include_fee
        description: Absorb the fee into the displayed cost
        type: query
      - in: query
        name: ticket_class.maximum_quantity
        description: Maximum number per order (blank for unlimited)
        type: query
      - in: query
        name: ticket_class.minimum_quantity
        description: Minimum number per order
        type: query
      - in: query
        name: ticket_class.name
        description: Name of this ticket type
        type: query
      - in: query
        name: ticket_class.order_confirmation_message
        description: Order message per ticket type
        type: query
      - in: query
        name: ticket_class.quantity_total
        description: Total available number of this ticket, required for non-donation
          tickets
        type: query
      - in: query
        name: ticket_class.sales_channels
        description: A list of all supported sales channels ([&#8220;online&#8221;],
          [&#8220;online&#8221;, &#8220;atd&#8221;], [&#8220;atd&#8221;])
        type: query
      - in: query
        name: ticket_class.sales_end
        description: When the ticket stops being on sale (leave empty for &#8216;one
          hour before event start&#8217;)
        type: query
      - in: query
        name: ticket_class.sales_start
        description: When the ticket is available for sale (leave empty for &#8216;when
          event published&#8217;)
        type: query
      - in: query
        name: ticket_class.sales_start_after
        description: The ID of another ticket class - when it sells out, this class
          will go on sale
        type: query
      - in: query
        name: ticket_class.split_fee
        description: Absorb the payment fee, but show the eventbrite fee
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
      - :ticket
      - Class
    delete:
      summary: Delete Events Ticket Classes Ticket Class
      description: 'Deletes the ticket class. Returns {&quot;deleted&quot;: true}.'
      operationId: deleteEventsTicketClassesTicketClass
      x-api-path-slug: eventsidticket-classesticket-class-id-delete
      parameters:
      - in: query
        name: break_dependency
        description: Delete even if ticket sales depend on this ticket
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Classes
      - :ticket
      - Class
  /events/{id}/canned_questions/:
    get:
      summary: Get Events Canned Questions
      description: 'This endpoint returns canned questions of a single event (examples:
        first name, last name, company, prefix, etc.). This endpoint will return question.'
      operationId: getEventsCannedQuestions
      x-api-path-slug: eventsidcanned-questions-get
      parameters:
      - in: query
        name: as_owner
        description: Return private events and more details
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Canned
      - Questions
    post:
      summary: Post Events Canned Questions
      description: Creates a new canned question; returns the result as a question.
      operationId: postEventsCannedQuestions
      x-api-path-slug: eventsidcanned-questions-post
      parameters:
      - in: query
        name: question.canned_type
        description: String value of canned_type
        type: query
      - in: query
        name: question.choices
        description: Choices for multiple choice questions
        type: query
      - in: query
        name: question.display_answer_on_order
        description: Is this question displayed on order confirmation?
        type: query
      - in: query
        name: question.parent_choice_id
        description: ID of Parent Question (for subquestions)
        type: query
      - in: query
        name: question.question.html
        description: Question displayed to the recipient
        type: query
      - in: query
        name: question.required
        description: Is an answer to this question required for registration?
        type: query
      - in: query
        name: question.respondent
        description: 'Ask this question to the ticket buyer or each attendee? (Valid
          choices are: ticket_buyer, or attendee)'
        type: query
      - in: query
        name: question.ticket_classes
        description: Tickets to which to limit this question
        type: query
      - in: query
        name: question.type
        description: 'Type of Question (Valid choices are: checkbox, dropdown, text,
          paragraph, radio, or waiver)'
        type: query
      - in: query
        name: question.waiver
        description: Waiver content for questions of type waiver
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Canned
      - Questions
  /events/{id}/questions/:
    get:
      summary: Get Events Questions
      description: |-
        Eventbrite allows event organizers to add custom questions that attendees fill
        out upon registration. This endpoint can be helpful for determining what
        custom information is collected and available per event.
      operationId: getEventsQuestions
      x-api-path-slug: eventsidquestions-get
      parameters:
      - in: query
        name: as_owner
        description: Return private events and more details
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Questions
    post:
      summary: Post Events Questions
      description: Creates a new question; returns the result as a question as the
        key question.
      operationId: postEventsQuestions
      x-api-path-slug: eventsidquestions-post
      parameters:
      - in: query
        name: question.choices
        description: Choices for multiple choice questions
        type: query
      - in: query
        name: question.display_answer_on_order
        description: Is this question displayed on order confirmation?
        type: query
      - in: query
        name: question.parent_choice_id
        description: ID of Parent Question Choice (for subquestions)
        type: query
      - in: query
        name: question.parent_id
        description: ID of Parent Question (for subquestions)
        type: query
      - in: query
        name: question.question.html
        description: Question displayed to the recipient
        type: query
      - in: query
        name: question.required
        description: Is an answer to this question required for registration?
        type: query
      - in: query
        name: question.respondent
        description: 'Ask this question to the ticket buyer or each attendee? (Valid
          choices are: ticket_buyer, or attendee)'
        type: query
      - in: query
        name: question.ticket_classes
        description: Tickets to which to limit this question
        type: query
      - in: query
        name: question.type
        description: 'Type of Question (Valid choices are: checkbox, dropdown, text,
          paragraph, radio, or waiver)'
        type: query
      - in: query
        name: question.waiver
        description: Waiver content for questions of type waiver
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Questions
  /events/{id}/questions/{id}/:
    get:
      summary: Get Events Questions
      description: This endpoint will return question for a specific question id.
      operationId: getEventsQuestions
      x-api-path-slug: eventsidquestionsid-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Questions
  /events/{id}/attendees/:attendee_id/:
    get:
      summary: Get Events Attendees Attendee
      description: Returns a single attendee by ID, as the key attendee.
      operationId: getEventsAttendeesAttendee
      x-api-path-slug: eventsidattendeesattendee-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Attendees
      - :attendee
  /events/{id}/orders/:
    get:
      summary: Get Events Orders
      description: Returns a paginated response with a key of orders, containing a
        list of order against this event.
      operationId: getEventsOrders
      x-api-path-slug: eventsidorders-get
      parameters:
      - in: query
        name: changed_since
        description: Only return orders changed on or after the time given
        type: query
      - in: query
        name: exclude_emails
        description: Don&#8217;t include orders placed by any of these emails
        type: query
      - in: query
        name: last_item_seen
        description: Only return orders changed on or after the time given and with
          an id bigger than last item seen
        type: query
      - in: query
        name: only_emails
        description: Only include orders placed by one of these emails
        type: query
      - in: query
        name: refund_request_statuses
        description: Return only orders with selected refund requests statuses
        type: query
      - in: query
        name: status
        description: 'Filter to active (attending), inactive (not attending), all
          (both) orders and all_not_deleted (active and inactive but not deleted)
          (Valid choices are: active, inactive, all, or all_not_deleted)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Orders
  /events/{id}/discounts/:
    get:
      summary: Get Events Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsDiscounts
      x-api-path-slug: eventsiddiscounts-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
    post:
      summary: Post Events Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsDiscounts
      x-api-path-slug: eventsiddiscounts-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
  /events/{id}/discounts/:discount_id/:
    get:
      summary: Get Events Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
      - :discount
    post:
      summary: Post Events Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
      operationId: postEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
      - :discount
    delete:
      summary: Delete Events Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsDiscountsDiscount
      x-api-path-slug: eventsiddiscountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Discounts
      - :discount
  /events/{id}/public_discounts/:
    get:
      summary: Get Events Public Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsPublicDiscounts
      x-api-path-slug: eventsidpublic-discounts-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
    post:
      summary: Post Events Public Discounts
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsPublicDiscounts
      x-api-path-slug: eventsidpublic-discounts-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
  /events/{id}/public_discounts/:discount_id/:
    get:
      summary: Get Events Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
      - :discount
    post:
      summary: Post Events Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id
      operationId: postEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
      - :discount
    delete:
      summary: Delete Events Public Discounts Discount
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsPublicDiscountsDiscount
      x-api-path-slug: eventsidpublic-discountsdiscount-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Public
      - Discounts
      - :discount
  /events/{id}/access_codes/:
    get:
      summary: Get Events Access Codes
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts
      operationId: getEventsAccessCodes
      x-api-path-slug: eventsidaccess-codes-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
    post:
      summary: Post Events Access Codes
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts
      operationId: postEventsAccessCodes
      x-api-path-slug: eventsidaccess-codes-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
    delete:
      summary: Delete Events Access Codes
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id
      operationId: deleteEventsAccessCodes
      x-api-path-slug: eventsidaccess-codes-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
  /events/{id}/access_codes/:access_code_id/:
    get:
      summary: Get Events Access Codes Access Code
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: getEventsAccessCodesAccessCode
      x-api-path-slug: eventsidaccess-codesaccess-code-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
      - :access
      - Code
    post:
      summary: Post Events Access Codes Access Code
      description: Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id
      operationId: postEventsAccessCodesAccessCode
      x-api-path-slug: eventsidaccess-codesaccess-code-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - Access
      - Codes
      - :access
      - Code
  /events/{id}/transfers/:
    get:
      summary: Get Events Transfers
      description: Returns a list of transfers for the event.
      operationId: getEventsTransfers
      x-api-path-slug: eventsidtransfers-get
      parameters:
      - in: query
        name: changed_since
        description: Only return transfers changed on or after the time given
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Transfers
  /events/{id}/teams/:
    get:
      summary: Get Events Teams
      description: Returns a list of attendee-team for the event.
      operationId: getEventsTeams
      x-api-path-slug: eventsidteams-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
  /events/{id}/teams/{id}/:
    get:
      summary: Get Events Teams
      description: Returns information for a single attendee-team.
      operationId: getEventsTeams
      x-api-path-slug: eventsidteamsid-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
  /events/{id}/teams/{id}/attendees/:
    get:
      summary: Get Events Teams Attendees
      description: Returns attendee for a single attendee-team.
      operationId: getEventsTeamsAttendees
      x-api-path-slug: eventsidteamsidattendees-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
      - Attendees
  /events/:event_id/ticket_groups/:
    get:
      summary: Get Events Event Ticket Groups
      description: |-
        Get the list of ticket_group for the event with the specified :event_id.
        By default, only the ticket groups that are live are shown.
      operationId: getEventsEventTicketGroups
      x-api-path-slug: eventsevent-idticket-groups-get
      parameters:
      - in: query
        name: status
        description: 'Limits results to groups with the specific status (Valid choices
          are: live, archived, deleted, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Groups
  /events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:ticket_group_id/:
    post:
      summary: Post Events Event Ticket Classes Ticket Class Ticket Groups Ticket
        Group
      description: Add the Ticket Class with the specified :ticket_class_id that belongs
        to the event with :event_id to the Ticket Group identified by :ticket_group_id.
      operationId: postEventsEventTicketClassesTicketClassTicketGroupsTicketGroup
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-post
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
      - :ticket
      - Group
    delete:
      summary: Delete Events Event Ticket Classes Ticket Class Ticket Groups Ticket
        Group
      description: Remove the Ticket Class with the specified :ticket_class_id that
        belongs to the event with :event_id from the Ticket Group identified by :ticket_group_id.
      operationId: deleteEventsEventTicketClassesTicketClassTicketGroupsTicketGroup
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groupsticket-group-id-delete
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
      - :ticket
      - Group
  /events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:
    get:
      summary: Get Events Event Ticket Classes Ticket Class Ticket Groups
      description: |-
        Get the Ticket Groups for Ticket Class with the specified :ticket_class_id that belongs to the event with :event_id.
        By default, only the ticket groups that are live are shown.
      operationId: getEventsEventTicketClassesTicketClassTicketGroups
      x-api-path-slug: eventsevent-idticket-classesticket-class-idticket-groups-get
      parameters:
      - in: query
        name: status
        description: 'Limits results to groups with the specific status (Valid choices
          are: live, archived, deleted, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
  /events/{id}/ticket_buyer_settings/:
    get:
      summary: Get Events Ticket Buyer Settings
      description: Returns a ticket_buyer_settings for an event.
      operationId: getEventsTicketBuyerSettings
      x-api-path-slug: eventsidticket-buyer-settings-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Buyer
      - Settings
    post:
      summary: Post Events Ticket Buyer Settings
      description: Updates the ticket buyer settings for an event. Returns a ticket_buyer_settings.
      operationId: postEventsTicketBuyerSettings
      x-api-path-slug: eventsidticket-buyer-settings-post
      parameters:
      - in: query
        name: ticket_buyer_settings.confirmation_message.html
        description: Confirmation message to display on order completion
        type: query
      - in: query
        name: ticket_buyer_settings.instructions.html
        description: Instructions to display on the ticket
        type: query
      - in: query
        name: ticket_buyer_settings.redirect_url
        description: Redirect to this url post-purchase
        type: query
      - in: query
        name: ticket_buyer_settings.refund_request_enabled
        description: Whether refund requests are accepted for the event
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ticket
      - Buyer
      - Settings
  /organizers/{id}/events/:
    get:
      summary: Get Organizers Events
      description: Gets events of the organizer.
      operationId: getOrganizersEvents
      x-api-path-slug: organizersidevents-get
      parameters:
      - in: query
        name: only_public
        description: Only show public events even if viewing your own events
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, or created_desc)'
        type: query
      - in: query
        name: start_date.range_end
        description: Only return events with start dates before the given date
        type: query
      - in: query
        name: start_date.range_start
        description: Only return events with start dates after the given date
        type: query
      - in: query
        name: status
        description: Only return events with a specific status set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - Events
  /events/:event_id/tracking_beacons/:
    get:
      summary: Get Events Event Tracking Beacons
      description: Returns the list of tracking_beacon for the event :event_id
      operationId: getEventsEventTrackingBeacons
      x-api-path-slug: eventsevent-idtracking-beacons-get
      parameters:
      - in: query
        name: return_fmt
        description: returned format
        type: query
      responses:
        200:
          description: OK
      tags:
      - Events
      - :event
      - Tracking
      - Beacons
  /users/{id}/owned_events/:
    get:
      summary: Get Users Owned Events
      description: |-
        Returns a paginated response of events, under
        the key events, of all events the user owns (i.e. events they are organising)
      operationId: getUsersOwnedEvents
      x-api-path-slug: usersidowned-events-get
      parameters:
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, created_desc, name_asc, or name_desc)'
        type: query
      - in: query
        name: show_series_parent
        description: 'True: Will show parent of a serie instead of childrenFalse:
          Will show children of a serie (Default value)'
        type: query
      - in: query
        name: status
        description: Filter by events with a specific status set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Events
  /users/{id}/events/:
    get:
      summary: Get Users Events
      description: Returns a paginated response of events, under the key events, of
        all events the user has access to
      operationId: getUsersEvents
      x-api-path-slug: usersidevents-get
      parameters:
      - in: query
        name: currency_filter
        description: Filter event results by currency
        type: query
      - in: query
        name: event_group_id
        description: Filter event results by event_group_id
        type: query
      - in: query
        name: name_filter
        description: Filter event results by name
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, created_desc, name_asc, or name_desc)'
        type: query
      - in: query
        name: page_size
        description: Number of records in each page
        type: query
      - in: query
        name: show_series_parent
        description: 'True: Will show parent of a serie instead of childrenFalse:
          Will show children of a serie (Default value)'
        type: query
      - in: query
        name: status
        description: Filter by events with a specific status set
        type: query
      - in: query
        name: time_filter
        description: Limits results to either past or current &amp; future events
          / orders
        type: query
      - in: query
        name: venue_filter
        description: Filter event results by venue IDs
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Events
  /organizations/{id}/events/:
    post:
      summary: Post Organizations Events
      description: Creates new events objects under an organization and returns it
        as event.
      operationId: postOrganizationsEvents
      x-api-path-slug: organizationsidevents-post
      parameters:
      - in: query
        name: event.capacity
        description: Set specific capacity (if omitted, sums ticket capacities)
        type: query
      - in: query
        name: event.category_id
        description: The category (vertical) of the event
        type: query
      - in: query
        name: event.currency
        description: Event currency (3 letter code)
        type: query
      - in: query
        name: event.description.html
        description: The description on the event page
        type: query
      - in: query
        name: event.end.timezone
        description: End time timezone (Olson format)
        type: query
      - in: query
        name: event.end.utc
        description: The end time of the event
        type: query
      - in: query
        name: event.format_id
        description: The format (general type) of the event
        type: query
      - in: query
        name: event.hide_end_date
        description: Whether the end date should be hidden
        type: query
      - in: query
        name: event.hide_start_date
        description: Whether the start date should be hidden
        type: query
      - in: query
        name: event.invite_only
        description: Only invited users can see the event page
        type: query
      - in: query
        name: event.is_reserved_seating
        description: If the event is reserved seating
        type: query
      - in: query
        name: event.listed
        description: If the event is publicly listed and searchable
        type: query
      - in: query
        name: event.logo.id
        description: (Deprecated) The logo for the event
        type: query
      - in: query
        name: event.logo_id
        description: The logo for the event
        type: query
      - in: query
        name: event.name.html
        description: The name of the event
        type: query
      - in: query
        name: event.online_event
        description: Is the event online-only (no venue)?
        type: query
      - in: query
        name: event.organizer_id
        description: The ID of the organizer of this event
        type: query
      - in: query
        name: event.password
        description: Password needed to see the event in unlisted mode
        type: query
      - in: query
        name: event.shareable
        description: If users can share the event on social media
        type: query
      - in: query
        name: event.show_pick_a_seat
        description: For reserved seating event, if attendees can pick their seats
        type: query
      - in: query
        name: event.show_remaining
        description: If the remaining number of tickets is publicly visible on the
          event page
        type: query
      - in: query
        name: event.show_seatmap_thumbnail
        description: For reserved seating event, if venue map thumbnail visible on
          the event page
        type: query
      - in: query
        name: event.source
        description: Source of the event (defaults to API)
        type: query
      - in: query
        name: event.start.timezone
        description: Start time timezone (Olson format)
        type: query
      - in: query
        name: event.start.utc
        description: The start time of the event
        type: query
      - in: query
        name: event.subcategory_id
        description: The subcategory of the event (US only)
        type: query
      - in: query
        name: event.venue_id
        description: ID of the venue
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Events
  /users/:user_id/events/:event_id/ticket_classes/:ticket_class_id/ticket_groups/:
    post:
      summary: Post Users User Events Event Ticket Classes Ticket Class Ticket Groups
      description: |-
        Add the Ticket Class with the specified :ticket_class_id of the event with :event_id that
        belongs to the user with :user_id to many Ticket Groups specified with ticket_group_ids.
        If the list provided is empty, remove this ticket class from every ticket group.
      operationId: postUsersUserEventsEventTicketClassesTicketClassTicketGroups
      x-api-path-slug: usersuser-ideventsevent-idticket-classesticket-class-idticket-groups-post
      parameters:
      - in: query
        name: ticket_group_ids
        description: IDs of all ticket group this ticket belongs to
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Events
      - :event
      - Ticket
      - Classes
      - :ticket
      - Class
      - Ticket
      - Groups
  /venues/{id}/events/:
    get:
      summary: Get Venues Events
      description: Returns events of a given venue.
      operationId: getVenuesEvents
      x-api-path-slug: venuesidevents-get
      parameters:
      - in: query
        name: only_public
        description: Only show public events even if viewing your own events
        type: query
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, or created_desc)'
        type: query
      - in: query
        name: start_date.range_end
        description: Only return events with start dates before the given date
        type: query
      - in: query
        name: start_date.range_start
        description: Only return events with start dates after the given date
        type: query
      - in: query
        name: status
        description: Only return events with a specific status set
        type: query
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Events
  /series/{id}/events/:
    get:
      summary: Get Series Events
      description: Returns all of the events that belong to this repeating event series.
      operationId: getSeriesEvents
      x-api-path-slug: seriesidevents-get
      parameters:
      - in: query
        name: order_by
        description: 'How to order the results (Valid choices are: start_asc, start_desc,
          created_asc, or created_desc)'
        type: query
      - in: query
        name: time_filter
        description: Limits results to either past or current &amp; future events
        type: query
      - in: query
        name: tracking_code
        description: Append the given tracking_code to the event URLs returned
        type: query
      responses:
        200:
          description: OK
      tags:
      - Series
      - Events
    post:
      summary: Post Series Events
      description: |-
        Creates more event dates or updates or deletes existing event dates in a repeating event series. In order for a series
        date to be deleted or updated, there must be no pending or completed orders for that date.
      operationId: postSeriesEvents
      x-api-path-slug: seriesidevents-post
      responses:
        200:
          description: OK
      tags:
      - Series
      - Events
  /user_list_events:
    get:
      summary: Get User List Events
      description: This method lists the events created by this user. Only public
        events are returned if no authentication is passed.
      operationId: Get_user_list_events_
      x-api-path-slug: user-list-events-get
      parameters:
      - in: query
        name: asc_or_desc
        description: Valid options include ???asc??? or results in ascending order
          or ???desc??? or descending order based on event start_date
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: do_not_display
        description: Comma separated list without spaces
      - in: query
        name: email
        description: The user email
      - in: query
        name: event_statuses
        description: Comma separated list without spaces
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Events
  /organizer_list_events:
    get:
      summary: Get Organizer List Events
      description: This method returns a list of events for a given organizer.
      operationId: Get_organizer_list_events_
      x-api-path-slug: organizer-list-events-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The organizer id
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - List
      - Events
  /users/{id}/owned_event_attendees/:
    get:
      summary: Get Users Owned Event Attendees
      description: |-
        Returns a paginated response of attendees,
        under the key attendees, of attendees visiting any of the events the user owns
        (events that would be returned from /users/:id/owned_events/)
      operationId: getUsersOwnedEventAttendees
      x-api-path-slug: usersidowned-event-attendees-get
      parameters:
      - in: query
        name: changed_since
        description: Only return resource changed on or after the time given
        type: query
      - in: query
        name: status
        description: Limits results to either confirmed attendees or cancelled/refunded/etc
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Event
      - Attendees
  /users/{id}/owned_event_orders/:
    get:
      summary: Get Users Owned Event Orders
      description: |-
        Returns a paginated response of orders,
        under the key orders, of orders placed against any of the events the user owns
        (events that would be returned from /users/:id/owned_events/)
      operationId: getUsersOwnedEventOrders
      x-api-path-slug: usersidowned-event-orders-get
      parameters:
      - in: query
        name: changed_since
        description: Only return resource changed on or after the time given
        type: query
      - in: query
        name: exclude_emails
        description: Don&#8217;t include orders placed by any of these emails
        type: query
      - in: query
        name: only_emails
        description: Only include orders placed by one of these emails
        type: query
      - in: query
        name: status
        description: 'Filter to active (attending), inactive (not attending), or all
          (both) orders (Valid choices are: active, inactive, or all)'
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Event
      - Orders
  /event_search:
    get:
      summary: Get Event Search
      description: This method uses our search index to find publicly listed events.
      operationId: Get_event_search_
      x-api-path-slug: event-search-get
      parameters:
      - in: query
        name: address
        description: The venue address
      - in: query
        name: category
        description: 'Event categories (comma seperated): conference, conventions,
          entertainment, fundraisers, meetings, other, performances, reunions, sales,
          seminars, social, sports, tradeshows, travel, religion, fairs, food, music,
          recreation'
      - in: query
        name: city
        description: The venue city
      - in: query
        name: country
        description: 2-letter country code, according to the ISO 3166 format
      - in: query
        name: count_only
        description: Only return the total number of events (???true??? or ???false???)
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: date
        description: The event start date
      - in: query
        name: date_created
        description: The date range the event was created, specified by a label or
          by exact dates
      - in: query
        name: date_modified
        description: The date range the event was modified, specified by a label or
          by exact dates
      - in: query
        name: keywords
        description: The search keywords
      - in: query
        name: latitude
        description: If ???within??? is set you can limit your search to wgs84 coordinates
          (latitude, longitude)
      - in: query
        name: longitude
        description: If ???within??? is set you can limit your search to wgs84 coordinates
          (latitude, longitude)
      - in: query
        name: max
        description: Limit the number of events returned
      - in: query
        name: organizer
        description: The organizer name
      - in: query
        name: page
        description: Allows for paging through the results of a query
      - in: query
        name: postal_code
        description: The postal/zip code of the venue
      - in: query
        name: region
        description: The venue state/province/county/territory depending on the country
      - in: query
        name: since_id
        description: Returns events with id greater than ???since_id??? value
      - in: query
        name: sort_by
        description: Sort the list of events by ???id???, ???date???, ???name???,
          ???city???
      - in: query
        name: tracking_link
        description: The tracking link code to add to the event URLs
      - in: query
        name: within
        description: If ???within??? is set and the ???city??? or ???zipcode??? resolve
          to a specific geolocation, the search will be restricted to the specified
          within radius
      - in: query
        name: within_unit
        description: 'If within is set, you can specify the unit to use: ???M??? for
          miles, or ???K??? for kilometers'
      responses:
        200:
          description: OK
      tags:
      - Event
      - Search
  /event_get:
    get:
      summary: Get Event Get
      description: This method returns the data for a given event. Only public events
        are viewable if no authentication is passed.
      operationId: Get_event_get_
      x-api-path-slug: event-get-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: event_id
        description: The ID of the requested event
      responses:
        200:
          description: OK
      tags:
      - Event
      - Get
  /event_new:
    get:
      summary: Get Event New
      description: This method creates a new event. It returns the ID of the newly
        created event.
      operationId: Get_event_new_
      x-api-path-slug: event-new-get
      parameters:
      - in: query
        name: background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_border_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: capacity
        description: The maximum number of people who can attend the event
      - in: query
        name: currency
        description: The event currency in ISO 4217 format (e
      - in: query
        name: custom_footer
        description: Custom HTML footer for your registration page
      - in: query
        name: custom_header
        description: Custom HTML header for your registration page
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The event description
      - in: query
        name: end_date
        description: The event end date and time, in ISO 8601 format (e
      - in: query
        name: organizer_id
        description: The event organizer ID
      - in: query
        name: personalized_url
        description: The event registration URL
      - in: query
        name: privacy
        description: 0 for a private event, 1 for a public event
      - in: query
        name: start_date
        description: The event start date and time, in ISO 8601 format (e
      - in: query
        name: status
        description: The event status
      - in: query
        name: text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: timezone
        description: The event time zone in relation to GMT (e
      - in: query
        name: title
        description: The event title
      - in: query
        name: title_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: venue_id
        description: The event venue ID
      responses:
        200:
          description: OK
      tags:
      - Event
      - New
  /event_update:
    get:
      summary: Get Event Update
      description: This method updates an existing event. Only the fields passed as
        arguments will be modified. This method returns the ID of the modified event.
      operationId: Get_event_update_
      x-api-path-slug: event-update-get
      parameters:
      - in: query
        name: background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_border_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_background_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_header_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: box_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: capacity
        description: The maximum number of people who can attend the event
      - in: query
        name: currency
        description: The event currency in ISO 4217 format (e
      - in: query
        name: custom_footer
        description: Custom HTML footer for your registration page
      - in: query
        name: custom_header
        description: Custom HTML header for your registration page
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: description
        description: The event description
      - in: query
        name: end_date
        description: The event end date and time, in ISO 8601 format (e
      - in: query
        name: event_id
        description: The ID of the event to update
      - in: query
        name: organizer_id
        description: The event organizer ID
      - in: query
        name: personalized_url
        description: The event registration URL subdomain
      - in: query
        name: privacy
        description: 0 for a private event, 1 for a public event
      - in: query
        name: start_date
        description: The event start date and time, in ISO 8601 format (e
      - in: query
        name: status
        description: The event status
      - in: query
        name: text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: timezone
        description: The event time zone in relation to GMT (e
      - in: query
        name: title
        description: The event title
      - in: query
        name: title_text_color
        description: Custom hexadecimal color for your registration page
      - in: query
        name: venue_id
        description: The event venue ID
      responses:
        200:
          description: OK
      tags:
      - Event
      - Update
  /event_copy:
    get:
      summary: Get Event Copy
      description: This method duplicates an existing event, returning the ID of the
        new event.
      operationId: Get_event_copy_
      x-api-path-slug: event-copy-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: event_id
        description: The ID of the existing event
      - in: query
        name: event_name
        description: A new name for this copy of the Event
      responses:
        200:
          description: OK
      tags:
      - Event
      - Copy
  /event_list_attendees:
    get:
      summary: Get Event List Attendees
      description: This method returns a list of attendees for a given event. If no
        authentication is passed, only publicly available attendee records will be
        returned.
      operationId: Get_event_list_attendees_
      x-api-path-slug: event-list-attendees-get
      parameters:
      - in: query
        name: count
        description: Limit the number of attendees returned
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: do_not_display
        description: Comma separated list without spaces that leaves out certain data
          returned
      - in: query
        name: event_id
        description: The ID of the event
      - in: query
        name: page
        description: Allows for paging through the results of a query
      - in: query
        name: show_full_barcodes
        description: If set to ???true???, it will return all barcodes associates
          with the attendee, plus the barcode status, device used, attendee_id, and
          barcode number
      responses:
        200:
          description: OK
      tags:
      - Event
      - List
      - Attendees
  /event_list_discounts:
    get:
      summary: Get Event List Discounts
      description: This method returns a list of discounts for a given event.
      operationId: Get_event_list_discounts_
      x-api-path-slug: event-list-discounts-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The ID of the event
      responses:
        200:
          description: OK
      tags:
      - Event
      - List
      - Discounts
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