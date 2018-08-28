swagger: "2.0"
x-collection-name: CollabNet
x-complete: 1
info:
  title: Foundation API
  version: 1.0.0
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