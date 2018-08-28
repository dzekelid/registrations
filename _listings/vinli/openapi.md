swagger: "2.0"
x-collection-name: Vinli
x-complete: 1
info:
  title: Vinli
  description: todo-add-description
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices:
    post:
      summary: Register a Device
      description: Register a device.
      operationId: DevicesPost
      x-api-path-slug: devices-post
      parameters:
      - in: header
        name: Accept
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
      - Device