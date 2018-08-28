---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Put Aps Ap
  description: Registers an APID. Unlike registration for iOS and BlackBerry applications,
    basic registration tying an APID to your application happens automatically. The
    registration API can be used to set aliases or tags. This returns HTTP 200 OK
    for any updates. Registering without any body is a no-op. Not including the alias
    field will clear it. To clear the list of tags, set it to the empty list []. If
    you are registering an APID to be used with C2DM, you will also need to include
    a C2DM registration ID.
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apids/{apid}:
    put:
      summary: Put Aps Ap
      description: Registers an APID. Unlike registration for iOS and BlackBerry applications,
        basic registration tying an APID to your application happens automatically.
        The registration API can be used to set aliases or tags. This returns HTTP
        200 OK for any updates. Registering without any body is a no-op. Not including
        the alias field will clear it. To clear the list of tags, set it to the empty
        list []. If you are registering an APID to be used with C2DM, you will also
        need to include a C2DM registration ID.
      operationId: apids.apid.put
      x-api-path-slug: apidsapid-put
      parameters:
      - in: query
        name: apid
        description: An APID (Android Push ID) is the Urban Airship ID of a device
          to which a message can be pushed
      - in: path
        name: apid
      - in: header
        name: Content-Type
        description: Content type
      - in: query
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Apids
      - Apid
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