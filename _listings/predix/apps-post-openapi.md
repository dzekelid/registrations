---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix AppHub ARCS Register the microapp
  description: Register the microapps
  termsOfService: Terms of service
  contact:
    name: 'Digital Predix AppHub ARCS: Development'
  version: 1.0.0
host: predix-apphub-arcs-prod.run.aws-usw02-pr.ice.predix.io
basePath: /api
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