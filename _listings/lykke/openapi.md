swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
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