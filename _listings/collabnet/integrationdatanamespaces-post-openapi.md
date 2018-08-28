---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Registers namespace
  version: 1.0.0
  description: Registers namespace.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /integrationdata/namespaces:
    post:
      summary: Registers namespace
      description: Registers namespace.
      operationId: registerNamespace
      x-api-path-slug: integrationdatanamespaces-post
      parameters:
      - in: body
        name: body
        description: Namespace
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Registers
      - Namespace
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