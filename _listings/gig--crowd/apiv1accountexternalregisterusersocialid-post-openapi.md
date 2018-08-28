---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Account External Register Usersocialid
  version: 1.0.0
  description: Post account external register usersocialid.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/account/register/org:
    post:
      summary: Post Account Register Org
      description: Post account register org.
      operationId: postApiV1AccountRegisterOrg
      x-api-path-slug: apiv1accountregisterorg-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Org
  /api/v1/account/register/art:
    post:
      summary: Post Account Register Art
      description: Post account register art.
      operationId: postApiV1AccountRegisterArt
      x-api-path-slug: apiv1accountregisterart-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Art
  /api/v1/account/register/invite:
    post:
      summary: Post Account Register Invite
      description: Post account register invite.
      operationId: postApiV1AccountRegisterInvite
      x-api-path-slug: apiv1accountregisterinvite-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Account
      - Register
      - Invite
  /api/v1/account/external/register/{userSocialId}:
    post:
      summary: Post Account External Register Usersocialid
      description: Post account external register usersocialid.
      operationId: postApiV1AccountExternalRegisterUsersocial
      x-api-path-slug: apiv1accountexternalregisterusersocialid-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userSocialId
        description: id UserSocial
      responses:
        200:
          description: OK
      tags:
      - Account
      - External
      - Register
      - Usersocialid
  /api/v1/gigme/account/register:
    post:
      summary: Post Gigme Account Register
      description: Post gigme account register.
      operationId: postApiV1GigmeAccountRegister
      x-api-path-slug: apiv1gigmeaccountregister-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Account
      - Register
  /api/v1/gigme/account/external/register/{userSocialId}:
    post:
      summary: Post Gigme Account External Register Usersocialid
      description: Post gigme account external register usersocialid.
      operationId: postApiV1GigmeAccountExternalRegisterUsersocial
      x-api-path-slug: apiv1gigmeaccountexternalregisterusersocialid-post
      parameters:
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: userSocialId
        description: id UserSocial
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Account
      - External
      - Register
      - Usersocialid
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