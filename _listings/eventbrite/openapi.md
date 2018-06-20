---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
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
  /users/:user_id/organizations/:
    get:
      summary: Get Users User Organizations
      description: |-
        Returns a continuated list of organizations
        accessible to the current user.
      operationId: getUsersUserOrganizations
      x-api-path-slug: usersuser-idorganizations-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - :user
      - Organizations
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
  /organizations/{id}/venues/:
    post:
      summary: Post Organizations Venues
      description: Creates new venue objects under an organization and returns it
        as venue.
      operationId: postOrganizationsVenues
      x-api-path-slug: organizationsidvenues-post
      parameters:
      - in: query
        name: venue.address.address_1
        description: The first line of the address
        type: query
      - in: query
        name: venue.address.address_2
        description: The second line of the address
        type: query
      - in: query
        name: venue.address.city
        description: The city where the venue is
        type: query
      - in: query
        name: venue.address.country
        description: The country where the venue is
        type: query
      - in: query
        name: venue.address.latitude
        description: The latitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.longitude
        description: The longitude of the coordinates for the venue
        type: query
      - in: query
        name: venue.address.postal_code
        description: The postal_code where the venue is
        type: query
      - in: query
        name: venue.address.region
        description: The region where the venue is
        type: query
      - in: query
        name: venue.age_restriction
        description: The age restrictions for the venue
        type: query
      - in: query
        name: venue.capacity
        description: The max capacity for the venue
        type: query
      - in: query
        name: venue.google_place_id
        description: The google place id for the venue
        type: query
      - in: query
        name: venue.name
        description: The name of the venue
        type: query
      - in: query
        name: venue.organizer_id
        description: The organizer this venue belongs to (optional - leave this off
          to use the default organizer)
        type: query
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Venues
---