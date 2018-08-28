swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 1
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resellernotify/register:
    post:
      summary: Register Reseller
      description: Registers a Reseller for receiving notifications.
      operationId: reseller.resellernotify.register
      x-api-path-slug: resellernotifyregister-post
      parameters:
      - in: query
        name: serviceAccountEmailAddress
        description: The service account which will own the created Cloud-PubSub topic
      responses:
        200:
          description: OK
      tags:
      - Register
  /resellernotify/unregister:
    post:
      summary: Unregister Reseller
      description: Unregisters a Reseller for receiving notifications.
      operationId: reseller.resellernotify.unregister
      x-api-path-slug: resellernotifyunregister-post
      parameters:
      - in: query
        name: serviceAccountEmailAddress
        description: The service account which owns the Cloud-PubSub topic
      responses:
        200:
          description: OK
      tags:
      - Register