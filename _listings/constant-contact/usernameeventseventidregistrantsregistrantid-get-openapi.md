---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Get Registrant
  description: Get Registrant
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/events/{event-id}/registrants/{registrant-id}:
    get:
      summary: Get Registrant
      description: Get Registrant
      operationId: get-registrant
      x-api-path-slug: usernameeventseventidregistrantsregistrantid-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Registrant
  /{username}/events/{event-id}/registrants:
    get:
      summary: List Registrants
      description: List Registrants
      operationId: list-registrants
      x-api-path-slug: usernameeventseventidregistrants-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Registrants
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