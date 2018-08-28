swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    get:
      summary: Get Events
      description: List public events.
      operationId: list-public-events
      x-api-path-slug: events-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      responses:
        200:
          description: OK
      tags:
      - Events
  /networks/{owner}/{repo}/events:
    get:
      summary: Get Networks Owner Repo Events
      description: List public events for a network of repositories.
      operationId: list-public-events-for-a-network-of-repositories
      x-api-path-slug: networksownerrepoevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of the owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Networks
      - Owner
      - Repo
      - Events
  /orgs/{org}/events:
    get:
      summary: Get Orgs Org Events
      description: List public events for an organization.
      operationId: list-public-events-for-an-organization
      x-api-path-slug: orgsorgevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: org
        description: Name of organisation
      responses:
        200:
          description: OK
      tags:
      - Orgs
      - Org
      - Events
  /repos/{owner}/{repo}/events:
    get:
      summary: Get Repos Owner Repo Events
      description: Get list of repository events.
      operationId: get-list-of-repository-events
      x-api-path-slug: reposownerrepoevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Events
  /repos/{owner}/{repo}/issues/events:
    get:
      summary: Get Repos Owner Repo Issues Events
      description: List issue events for a repository.
      operationId: list-issue-events-for-a-repository
      x-api-path-slug: reposownerrepoissuesevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Events
  /repos/{owner}/{repo}/issues/events/{eventId}:
    get:
      summary: Get Repos Owner Repo Issues Events Event
      description: Get a single event.
      operationId: get-a-single-event
      x-api-path-slug: reposownerrepoissueseventseventid-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: eventId
        description: Id of the event
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Events
      - Event
  /repos/{owner}/{repo}/issues/{number}/events:
    get:
      summary: Get Repos Owner Repo Issues Number Events
      description: List events for an issue.
      operationId: list-events-for-an-issue
      x-api-path-slug: reposownerrepoissuesnumberevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: number
        description: Number of issue
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Issues
      - Number
      - Events
  /users/{username}/events:
    get:
      summary: Get Users Username Events
      description: If you are authenticated as the given user, you will see your private
        events. Otherwise, you'll only see public events.
      operationId: if-you-are-authenticated-as-the-given-user-you-will-see-your-private-events-otherwise-youll-only-see
      x-api-path-slug: usersusernameevents-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Events
  /users/{username}/events/orgs/{org}:
    get:
      summary: Get Users Username Events Orgs Org
      description: This is the user's organization dashboard. You must be authenticated
        as the user to view this.
      operationId: this-is-the-users-organization-dashboard-you-must-be-authenticated-as-the-user-to-view-this
      x-api-path-slug: usersusernameeventsorgsorg-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: org
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Events
      - Orgs
      - Org
  /users/{username}/received_events:
    get:
      summary: Get Users Username Received Events
      description: These are events that you'll only see public events.
      operationId: these-are-events-that-youll-only-see-public-events
      x-api-path-slug: usersusernamereceived-events-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Received
      - Events
  /users/{username}/received_events/public:
    get:
      summary: Get Users Username Received Events Public
      description: List public events that a user has received
      operationId: list-public-events-that-a-user-has-received
      x-api-path-slug: usersusernamereceived-eventspublic-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: username
        description: Name of user
      responses:
        200:
          description: OK
      tags:
      - Users
      - Username
      - Received
      - Events
      - Public