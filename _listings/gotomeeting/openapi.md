---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: Go To Training
  description: the-gototraining-api-enables-developers-to-use-the-stable-and-robust-gototraining-functionality-as-the-basis-for-online-trainings-in-a-proprietary-learning-management-system--the-gototraining-apis-provide-the-ability-to-access-the-scheduling-registration-management-and-reporting-functions-of-gototraining-from-external-applications--with-the-ability-to-tightly-integrate-gototraining-into-your-learning-infrastructure-you-can-offer-your-learners-a-seamless-user-experience-and-provide-them-with-a-market-leading-virtual-classroom-environment-
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
---