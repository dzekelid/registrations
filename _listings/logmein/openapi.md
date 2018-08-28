swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
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
  /{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}:
    get:
      summary: Get Registrant
      description: Get registrant.
      operationId: WebinarsRegistrantsRegistrantKeyByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeyregistrantsregistrantkey-get
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
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Registrant
    delete:
      summary: Delete Registrant
      description: Delete registrant.
      operationId: WebinarsRegistrantsRegistrantKeyByOrganizerKeyAndWebinarKeyDelete
      x-api-path-slug: organizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
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
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Registrant
  /{organizerKey}/webinars/{webinarKey}/registrants:
    post:
      summary: Create Registrant (Version 2)
      description: Create registrant (version 2).
      operationId: WebinarsRegistrantsByOrganizerKeyAndWebinarKeyPost2
      x-api-path-slug: organizerkeywebinarswebinarkeyregistrants-post
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
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Registrant
      - (Version
      - 2)
    get:
      summary: Get registrants
      description: Get registrants.
      operationId: WebinarsRegistrantsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeyregistrants-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Registrants
  /{organizerKey}/webinars/{webinarKey}/registrants/fields:
    get:
      summary: Get registration fields
      description: Get registration fields.
      operationId: WebinarsRegistrantsFieldsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeyregistrantsfields-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Registration
      - Fields