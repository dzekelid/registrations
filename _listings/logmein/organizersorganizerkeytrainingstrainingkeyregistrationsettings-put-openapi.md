---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToTraining Update Training Registration Settings
  description: Update training registration settings.
  version: 1.0.0
host: api.getgo.com
basePath: /G2T/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers/{organizerKey}/trainings/{trainingKey}/registrants/{registrantKey}:
    get:
      summary: Get Registrant
      description: Get registrant.
      operationId: OrganizersTrainingsRegistrantsRegistrantKeyByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Registrant
    delete:
      summary: Cancel Registration
      description: Cancel registration.
      operationId: OrganizersTrainingsRegistrantsRegistrantKeyByOrganizerKeyAndTrainingKeyDelete
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Registration
  '/organizers/{organizerKey}/trainings/{trainingKey}/registrants ':
    get:
      summary: Get Training Registrants
      description: Get training registrants.
      operationId: OrganizersTrainingsRegistrantsByOrganizerKeyAndTrainingKeyGet
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
      - Registrants
    post:
      summary: Register for Training
      description: Register for training.
      operationId: OrganizersTrainingsRegistrantsByOrganizerKeyAndTrainingKeyPost
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - RegisterTraining
  /organizers/{organizerKey}/trainings/{trainingKey}/registrationSettings:
    put:
      summary: Update Training Registration Settings
      description: Update training registration settings.
      operationId: OrganizersTrainingsRegistrationSettingsByOrganizerKeyAndTrainingKeyPut
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: trainingKey
      responses:
        200:
          description: OK
      tags:
      - Training
      - Registration
      - Settings
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