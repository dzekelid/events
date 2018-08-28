---
swagger: "2.0"
x-collection-name: Bitbucket
x-complete: 1
info:
  title: Bitbucket
  description: code-against-the-bitbucket-api-to-automate-simple-tasks-embed-bitbucket-data-into-your-own-site-build-mobile-or-desktop-apps-or-even-add-custom-ui-addons-into-bitbucket-itself-using-the-connect-framework-
  termsOfService: https://www.atlassian.com/legal/customer-agreement
  contact:
    name: Bitbucket Support
    url: https://support.atlassian.com/bitbucket
    email: support@bitbucket.org
  version: 1.0.0
host: api.bitbucket.org
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /hook_events:
    get:
      summary: Get Hook Events
      description: |-
        Returns the webhook resource or subject types on which webhooks can
        be registered.

        Each resource/subject type contains an `events` link that returns the
        paginated list of specific events each individual subject type can
        emit.

        This endpoint is publicly accessible and does not require
        authentication or scopes.

        Example:

        ```
        $ curl https://api.bitbucket.org/2.0/hook_events

        {
            "repository": {
                "links": {
                    "events": {
                        "href": "https://api.bitbucket.org/2.0/hook_events/repository"
                    }
                }
            },
            "team": {
                "links": {
                    "events": {
                        "href": "https://api.bitbucket.org/2.0/hook_events/team"
                    }
                }
            },
            "user": {
                "links": {
                    "events": {
                        "href": "https://api.bitbucket.org/2.0/hook_events/user"
                    }
                }
            }
        }
        ```
      operationId: getHookEvents
      x-api-path-slug: hook-events-get
      responses:
        200:
          description: OK
      tags:
      - Hook
      - Events
    parameters:
      summary: Parameters Hook Events
      description: Parameters hook events
      operationId: parametersHookEvents
      x-api-path-slug: hook-events-parameters
      responses:
        200:
          description: OK
      tags:
      - Hook
      - Events
  /hook_events/{subject_type}:
    get:
      summary: Get Hook Events Subject Type
      description: |-
        Returns a paginated list of all valid webhook events for the
        specified entity.

        This is public data that does not require any scopes or authentication.

        Example:

        NOTE: The following example is a truncated response object for the `team` `subject_type`.
        We return the same structure for the other `subject_type` objects.

        ```
        $ curl https://api.bitbucket.org/2.0/hook_events/team
        {
            "page": 1,
            "pagelen": 30,
            "size": 21,
            "values": [
                {
                    "category": "Repository",
                    "description": "Whenever a repository push occurs",
                    "event": "repo:push",
                    "label": "Push"
                },
                {
                    "category": "Repository",
                    "description": "Whenever a repository fork occurs",
                    "event": "repo:fork",
                    "label": "Fork"
                },
                ...
                {
                    "category": "Repository",
                    "description": "Whenever a repository import occurs",
                    "event": "repo:imported",
                    "label": "Import"
                }
            ]
        }
        ```
      operationId: getHookEventsSubjectType
      x-api-path-slug: hook-eventssubject-type-get
      parameters:
      - in: path
        name: subject_type
        description: A resource or subject type
      responses:
        200:
          description: OK
      tags:
      - Hook
      - Events
      - Subject
      - Type
    parameters:
      summary: Parameters Hook Events Subject Type
      description: Parameters hook events subject type
      operationId: parametersHookEventsSubjectType
      x-api-path-slug: hook-eventssubject-type-parameters
      responses:
        200:
          description: OK
      tags:
      - Hook
      - Events
      - Subject
      - Type
---