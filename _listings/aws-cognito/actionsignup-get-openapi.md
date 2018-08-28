---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 0
info:
  title: AWS Cognito API Sign Up
  version: 1.0.0
  description: |-
    Registers the user in the specified user pool and creates a user name, password,
                and user attributes.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetOpenIdTokenForDeveloperIdentity:
    get:
      summary: Get Open Id Token For Developer Identity
      description: |-
        Registers (or retrieves) a Cognito IdentityId and an OpenID Connect
                 token for a user authenticated by your backend authentication process.
      operationId: getOpenIdTokenForDeveloperIdentity
      x-api-path-slug: actiongetopenidtokenfordeveloperidentity-get
      parameters:
      - in: query
        name: IdentityId
        description: A unique identifier in the format REGION:GUID
        type: string
      - in: query
        name: IdentityPoolId
        description: An identity pool ID in the format REGION:GUID
        type: string
      - in: query
        name: Logins
        description: A set of optional name-value pairs that map provider names to
          provider tokens
        type: string
      - in: query
        name: TokenDuration
        description: The expiration time of the token, in seconds
        type: string
      responses:
        200:
          description: OK
      tags:
      - Open ID Token for Developer Identities
  /?Action=RegisterDevice:
    get:
      summary: Register Device
      description: Registers a device to receive push sync notifications.
      operationId: registerDevice
      x-api-path-slug: actionregisterdevice-get
      parameters:
      - in: query
        name: IdentityId
        description: The unique ID for this identity
        type: string
      - in: query
        name: IdentityPoolId
        description: A name-spaced GUID (for example, us-east-1:23EC4050-6AEA-7089-A2DD-08002EXAMPLE)
          created by Amazon Cognito
        type: string
      responses:
        200:
          description: OK
      tags:
      - Devices
  /?Action=SignUp:
    get:
      summary: Sign Up
      description: |-
        Registers the user in the specified user pool and creates a user name, password,
                    and user attributes.
      operationId: signUp
      x-api-path-slug: actionsignup-get
      parameters:
      - in: query
        name: ClientId
        description: The ID of the client associated with the user pool
        type: string
      - in: query
        name: Password
        description: The password of the user you wish to register
        type: string
      - in: query
        name: SecretHash
        description: A keyed-hash message authentication code (HMAC) calculated using
          the secret key of            a user pool client and username plus the client
          ID in the message
        type: string
      - in: query
        name: UserAttributes
        description: An array of name-value pairs representing user attributes
        type: string
      - in: query
        name: Username
        description: The user name of the user you wish to register
        type: string
      - in: query
        name: ValidationData
        description: The validation data in the request to register a user
        type: string
      responses:
        200:
          description: OK
      tags:
      - Sign Up
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