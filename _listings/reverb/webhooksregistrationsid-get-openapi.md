---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: reverb Get Webhooks Registrations
  description: Get details of a webhook registration
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /webhooks/registrations:
    get:
      summary: Get Webhooks Registrations
      description: Get webhooks registrations.
      operationId: getWebhooksRegistrations
      x-api-path-slug: webhooksregistrations-get
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Registrations
    post:
      summary: Post Webhooks Registrations
      description: Post webhooks registrations.
      operationId: postWebhooksRegistrations
      x-api-path-slug: webhooksregistrations-post
      parameters:
      - in: body
        name: body
        description: the content of the request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Registrations
  /webhooks/registrations/{id}:
    delete:
      summary: Delete Webhooks Registrations
      description: Delete webhooks registrations.
      operationId: deleteWebhooksRegistrations
      x-api-path-slug: webhooksregistrationsid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Registrations
      - Id
    get:
      summary: Get Webhooks Registrations
      description: Get details of a webhook registration
      operationId: getWebhooksRegistrations
      x-api-path-slug: webhooksregistrationsid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Webhooks
      - Registrations
      - Id
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