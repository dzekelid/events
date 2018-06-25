---
name: Bitbucket
x-slug: bitbucket
description: Collaborate on code with inline comments and pull requests. Manage and
  share your Git repositories to build and ship software, as a team.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
x-kinRank: "8"
x-alexaRank: "901"
tags: Events
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/apis.md
specificationVersion: "0.14"
apis:
- name: Bitbucket Get Hook Events
  x-api-slug: bitbucket
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//hook_events
  tags: Hook, Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/hook-events-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/hook-events-get-openapi.md
- name: Bitbucket Parameters Hook Events
  x-api-slug: bitbucket
  description: Parameters hook events
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//hook_events
  tags: Hook, Events
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/hook-events-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/hook-events-parameters-openapi.md
- name: Bitbucket Get Hook Events Subject Type
  x-api-slug: bitbucket
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//hook_events/{subject_type}
  tags: Hook, Events, Subject, Type
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/hook-eventssubject-type-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/hook-eventssubject-type-get-openapi.md
- name: Bitbucket Parameters Hook Events Subject Type
  x-api-slug: bitbucket
  description: Parameters hook events subject type
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0//hook_events/{subject_type}
  tags: Hook, Events, Subject, Type
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/hook-eventssubject-type-parameters-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/hook-eventssubject-type-parameters-openapi.md
- name: Bitbucket
  x-api-slug: bitbucket
  description: Collaborate on code with inline comments and pull requests. Manage
    and share your Git repositories to build and ship software, as a team.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19810-bitbucket.jpg
  humanURL: http://bitbucket.org
  baseURL: https://api.bitbucket.org//2.0
  tags: Events
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/events/master/_listings/bitbucket/openapi.md
x-common:
- type: x-crunchbase
  url: https://crunchbase.com/organization/bitbucket
- type: x-developer
  url: https://developer.atlassian.com/cloud/bitbucket/
- type: x-documentation
  url: https://confluence.atlassian.com/bitbucket/bitbucket-cloud-documentation-221448814.html?_ga=2.77295890.629375793.1519179030-1077111323.1516485126
- type: x-status
  url: https://status.bitbucket.org/?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-support
  url: https://support.atlassian.com/bitbucket-cloud/
- type: x-terms-of-service
  url: https://www.atlassian.com/legal/customer-agreement?_ga=2.76365714.629375793.1519179030-1077111323.1516485126
- type: x-twitter
  url: https://twitter.com/bitbucket
- type: x-website
  url: http://bitbucket.org
- type: x-website
  url: https://bitbucket.org/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---