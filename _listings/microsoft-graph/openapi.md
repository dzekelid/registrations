swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/{id}/registeredOwners:
    get:
      summary: List Registered Owners
      description: List registeredOwners Retrieve a list of users that are registered
        owners of the device.
      operationId: ListRegisteredOwners
      x-api-path-slug: devicesidregisteredowners-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Owners
    post:
      summary: Create Registered Owner
      description: Create registeredOwner Add a user as a registered owner of the
        device.
      operationId: CreateRegisteredOwner
      x-api-path-slug: devicesidregisteredowners-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Registered
      - Owner
  /devices/{id}/registeredUsers:
    get:
      summary: List Registered Users
      description: List registeredUsers Retrieve a list of users that are registered
        users of the device.
      operationId: ListRegisteredUsers
      x-api-path-slug: devicesidregisteredusers-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Users
    post:
      summary: Create Registered User
      description: Create registeredUser Add a registered user for the device.
      operationId: CreateRegisteredUser
      x-api-path-slug: devicesidregisteredusers-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Registered
      - User
  /users/{id | userPrincipalName}/registeredDevices:
    get:
      summary: List Registered Devices
      description: List registeredDevices Get the list of user's registered devices.
      operationId: ListRegisteredDevices
      x-api-path-slug: usersid--userprincipalnameregistereddevices-get
      parameters:
      - in: header
        name: Accept
        description: application/json
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Devices