swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
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