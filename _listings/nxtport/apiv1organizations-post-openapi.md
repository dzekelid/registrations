---
swagger: "2.0"
x-collection-name: NxtPort
x-complete: 0
info:
  title: NxtPort T-mining Secure Container Release API Register organization
  description: Register an Organization with a name. The name must be unique, so if
    one registers an Organization with a name that is already in use, an error will
    occur.
  contact:
    name: T-Mining API support
    url: http://support.t-mining.be/
    email: support@t-mining.be
  version: 1.0.0
host: api.nxtport.eu
basePath: /blockchain
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/organizations:
    post:
      summary: Register organization
      description: Register an Organization with a name. The name must be unique,
        so if one registers an Organization with a name that is already in use, an
        error will occur.
      operationId: postApiV1Organizations
      x-api-path-slug: apiv1organizations-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Register
      - Organization
  /api/v1/users:
    post:
      summary: Register user
      description: |-
        Register information of a user. Note that the "real" (human) user should have
        an account on the blockchain (upfront). This account is represented by an address on the chain, which is based on the public key of the user. Registering therefore means defining user **properties** like a username, which can then be used to refer to users in a more human-friendly way then by using the account addresses. User registration should be done by the user who owns an account on the chain. As a result of registration, a User contract is created on the chain, which contains the user properties, and which is owned by the user account. From then on, one can use the username to refer to a user on the web/mobile app.
      operationId: postApiV1Users
      x-api-path-slug: apiv1users-post
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Register
      - User
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