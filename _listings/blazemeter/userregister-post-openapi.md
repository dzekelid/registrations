---
swagger: "2.0"
x-collection-name: BlazeMeter
x-complete: 0
info:
  title: Blazemeter Post User Register
  description: Post user register.
  version: 1.0.0
host: a.blazemeter.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/register:
    get:
      summary: Get User Register
      description: Get user register.
      operationId: register_retrieve
      x-api-path-slug: userregister-get
      parameters:
      - in: query
        name: email
        description: Email address
      - in: query
        name: firstName
        description: First name
      - in: query
        name: lastName
        description: Last name
      - in: query
        name: password
        description: Password
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Register
    post:
      summary: Post User Register
      description: Post user register.
      operationId: register
      x-api-path-slug: userregister-post
      parameters:
      - in: body
        name: blazemeter\Routing\v4\UserModel4
        description: firstName (required)lastName (required)email (required)password
          (required)
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - User
      - Register
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