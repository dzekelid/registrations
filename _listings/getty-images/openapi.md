swagger: "2.0"
x-collection-name: Getty Images
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
  version: 1.0.0
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/asset-registrations:
    post:
      summary: Register Assets
      description: "# Register Assets\r\n\r\nRegisters a list of assets that a customer
        has stored in their system.\r\n\r\n##  Quickstart\r\n\r\nYou'll need an API
        key and a [Resource Owner Grant](http://developers.gettyimages.com/en/authorization-faq.html)
        access token to use this resource.\r\nPlease see our [Getting Started](http://developers.gettyimages.com/en/getting-started.html)
        page for more information on how to sign up for an API key. \r\n\r\n_Note_:
        In the event of a successful query (response code 200) there will be nothing
        in the response body."
      operationId: AssetRegistration_Register
      x-api-path-slug: v3assetregistrations-post
      parameters:
      - in: body
        name: request
        description: Specify JSON containing an array of asset ids to register
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Images
      - Registrations