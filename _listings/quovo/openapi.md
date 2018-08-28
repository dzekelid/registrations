swagger: "2.0"
x-collection-name: Quovo
x-complete: 1
info:
  title: Quovo API v3
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /webhooks:
    post:
      summary: Register a new webhook
      description: Used to register new webhooks.
      operationId: WebhooksPost
      x-api-path-slug: webhooks-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Register
      - New
      - Webhook
    get:
      summary: Get all registered webhooks
      description: "Retrieve your registered webhooks. \n\nNote: secret is intentionally
        omitted from all GET requests. It is only returned after being updated or
        after a new webhook is created."
      operationId: WebhooksGet
      x-api-path-slug: webhooks-get
      responses:
        200:
          description: OK
      tags:
      - Registered
      - Webhooks