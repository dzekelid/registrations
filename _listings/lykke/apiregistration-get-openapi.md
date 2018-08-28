---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API Registration
  version: 1.0.0
  description: Get api registration.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Registration:
    get:
      summary: Get API Registration
      description: Get api registration.
      operationId: ApiRegistrationGet
      x-api-path-slug: apiregistration-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Registration
    post:
      summary: Add API Registration
      description: Add api registration.
      operationId: ApiRegistrationPost
      x-api-path-slug: apiregistration-post
      parameters:
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Registration
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