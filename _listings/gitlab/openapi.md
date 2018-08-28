swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/events:
    get:
      summary: Get Projects Events
      description: Get events for a single project
      operationId: getV3ProjectsIdEvents
      x-api-path-slug: v3projectsidevents-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Events
  /v3/users/{id}/events:
    get:
      summary: Get Users Events
      description: This feature was introduced in GitLab 8.13.
      operationId: getV3UsersIdEvents
      x-api-path-slug: v3usersidevents-get
      parameters:
      - in: path
        name: id
        description: The ID of the user
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Users
      - Events