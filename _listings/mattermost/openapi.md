swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost
  version: 1.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /oauth/apps:
    post:
      summary: Register OAuth app
      description: |-
        Register an OAuth 2.0 client application with Mattermost as the service provider.
        ##### Permissions
        Must have `manage_oauth` permission.
      operationId: register-an-oauth-20-client-application-with-mattermost-as-the-service-provider-permissionsmust-have
      x-api-path-slug: oauthapps-post
      parameters:
      - in: body
        name: body
        description: OAuth application to register
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Register
      - OAuth
      - App