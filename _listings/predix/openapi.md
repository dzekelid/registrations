swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apps:
    post:
      summary: Register the microapp
      description: Register the microapps
      operationId: registerAppUsingPOST
      x-api-path-slug: apps-post
      parameters:
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Apps
  /v1/object/registerObject:
    post:
      summary: Register Object
      description: Register Object. A registered object can be queried from Query
        APIs.
      operationId: apply
      x-api-path-slug: v1objectregisterobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Register
      - Object
  /v1/object/registerGroup:
    post:
      summary: Register Object per Group
      description: Register Object per Group. A registered object can be queried from
        Query APIs.
      operationId: groupApply
      x-api-path-slug: v1objectregistergroup-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Register
      - Object
      - Per
      - Group
  /v1/object/deleteRegisteredObject:
    post:
      summary: Delete Registered Object
      description: Delete registered object.
      operationId: deleteRegularRegistration
      x-api-path-slug: v1objectdeleteregisteredobject-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - Registered
      - Object
  /v1/object/listObjects:
    post:
      summary: List Registered Objects
      description: List registered Objects.
      operationId: reference
      x-api-path-slug: v1objectlistobjects-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Objects
  /v1/registrations:
    post:
      summary: Post Registrations
      description: |-
        The following parameters can be used to validate the user's request.
        The parameters are optional, but the sample code includes email as part of the requestParams.post method.
      operationId: postV1Registrations
      x-api-path-slug: v1registrations-post
      parameters:
      - in: body
        name: body
        description: Body Parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Registrations
  /v1/registrations/{registration_id}:
    get:
      summary: Get Registrations
      description: You can use a registration_id to retrieve the respective registration
        object.
      operationId: getV1RegistrationsRegistration
      x-api-path-slug: v1registrationsregistration-id-get
      parameters:
      - in: path
        name: registration_id
      responses:
        200:
          description: OK
      tags:
      - Registrations