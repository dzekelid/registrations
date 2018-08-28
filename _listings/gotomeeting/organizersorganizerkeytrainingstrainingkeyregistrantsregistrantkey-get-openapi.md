---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: Go To Training Get Registrant
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2T/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers/{organizerKey}/trainings/{trainingKey}/registrants/{registrantKey}:
    delete:
      summary: Cancel Registration
      description: This call cancels a registration in a scheduled training for a
        specific registrant. If the registrant has paid for the training, a cancellation
        cannot be completed with this method; it must be completed on the external
        admin site. No notification is sent to the registrant or the organizer by
        default. The registrant can re-register if needed.
      operationId: cancelRegistration
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Trainings
      - TrainingKey
      - Registrants
      - RegistrantKey
    get:
      summary: Get Registrant
      description: 'Retrieves details for specific registrant in a specific training.
        Registrants can be:<br>WAITING - registrant registered and is awaiting approval
        (where organizer has required approval)<br>APPROVED - registrant registered
        and is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
        The registrant data caches are typically updated immediately and the data
        will be returned in the response. However, the update can take as long as
        two hours.'
      operationId: getRegistrant
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Trainings
      - TrainingKey
      - Registrants
      - RegistrantKey
  /organizers/{organizerKey}/trainings/{trainingKey}/registrants:
    get:
      summary: Get Training Registrants
      description: 'Retrieves details on all registrants for a specific training.
        Registrants can be:<br>WAITING - registrant registered and is awaiting approval
        (where organizer has required approval)<br>APPROVED - registrant registered
        and is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
        The registrant data caches are typically updated immediately and the data
        will be returned in the response. However, the update can take as long as
        two hours.'
      operationId: getRegistrants
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Trainings
      - TrainingKey
      - Registrants
    post:
      summary: Register for Training
      description: 'Registers one person, identified by a unique email address, for
        a training. Approval is automatic unless payment or approval is required.
        The response contains the Confirmation page URL and Join URL for the registrant.
        NOTE: If some registrants do not receive a confirmation email, the emails
        could be getting blocked by their email server due to spam filtering or a
        grey-listing setting.'
      operationId: registerForTraining
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
      parameters:
      - in: body
        name: body
        description: The details of the registrant to create
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Trainings
      - TrainingKey
      - Registrants
  /organizers/{organizerKey}/trainings/{trainingKey}/registrationSettings:
    put:
      summary: Update Training Registration Settings
      description: An API request to automatically enable or disable web registrations
        and confirmation emails to registrants.
      operationId: updateRegistrationSettingsForTraining
      x-api-path-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
      parameters:
      - in: body
        name: body
        description: The new registration settings for the training
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Trainings
      - TrainingKey
      - RegistrationSettings
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