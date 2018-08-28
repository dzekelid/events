---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Get Cognito Events
  version: 1.0.0
  description: Gets the events and the corresponding Lambda functions associated with
    an identity pool.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetCognitoEvents:
    get:
      summary: Get Cognito Events
      description: Gets the events and the corresponding Lambda functions associated
        with an identity pool.
      operationId: getCognitoEvents
      x-api-path-slug: actiongetcognitoevents-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: The Cognito Identity Pool ID for the request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
  /?Action=SetCognitoEvents:
    get:
      summary: Set Cognito Events
      description: Sets the AWS Lambda function for a given event type for an identity
        pool.
      operationId: setCognitoEvents
      x-api-path-slug: actionsetcognitoevents-get
      parameters:
      - in: query
        name: IdentityPoolId
        description: The Cognito Identity Pool to use when configuring Cognito Events
        type: string
      responses:
        200:
          description: OK
      tags:
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