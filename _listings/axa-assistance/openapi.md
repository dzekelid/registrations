swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 1
info:
  title: AXA Assistance
  description: axa-assistance-is-a-worldwide-specialist-for-car-insurance-travel-health-and-home-services--trust-in-axa-assistance-for-your-insurance
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/v1/identities/register/confirm:
    post:
      summary: Confirm identity registration
      description: Confirm identity registration
      operationId: postUserV1IdentitiesRegisterConfirm
      x-api-path-slug: userv1identitiesregisterconfirm-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Confirm
      - identity
      - registration
  /user/v1/identities/register/sendOTP:
    post:
      summary: SendOTP on registration
      description: SendOTP on registration
      operationId: postUserV1IdentitiesRegisterSendotp
      x-api-path-slug: userv1identitiesregistersendotp-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - SendOTP
      - "on"
      - registration
  /user/v1/identities/register:
    post:
      summary: Register identity
      description: Register identity
      operationId: postUserV1IdentitiesRegister
      x-api-path-slug: userv1identitiesregister-post
      parameters:
      - in: header
        name: accept-language
        description: Language/Country
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Register
      - identity