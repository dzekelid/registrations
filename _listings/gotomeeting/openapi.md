swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: SCIM
  description: the-scim-api-lets-you-manage-users-in-your-organization--you-can-then-automate-the-provisioning-of-product-licenses-for-these-users-and-they-can-use-your-companys-single-signon-solution-through-an-identity-provider-
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: N/A
host: api.citrixonline.com
basePath: /identity/v1
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
  /organizers/{organizerKey}/webinars/{webinarKey}/registrants/{registrantKey}:
    delete:
      summary: Delete registrant
      description: Removes a webinar registrant from current registrations for the
        specified webinar. The webinar must be a scheduled, future webinar.
      operationId: deleteRegistrant
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Registrants
      - RegistrantKey
    get:
      summary: Get registrant
      description: Retrieve registration details for a specific registrant.
      operationId: getRegistrant
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Registrants
      - RegistrantKey
  /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}:
    get:
      summary: Get attendee
      description: Retrieve registration details for a particular attendee of a specific
        webinar session. For technical reasons, this call cannot be executed from
        this documentation. Please use the curl command to execute it.
      operationId: getAttendee
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Sessions
      - SessionKey
      - Attendees
      - RegistrantKey
  /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/polls:
    get:
      summary: Get attendee poll answers
      description: Get poll answers from a particular attendee of a specific webinar
        session. For technical reasons, this call cannot be executed from this documentation.
        Please use the curl command to execute it.
      operationId: getAttendeePollAnswers
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Sessions
      - SessionKey
      - Attendees
      - RegistrantKey
      - Polls
  /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/questions:
    get:
      summary: Get attendee questions
      description: Get questions asked by an attendee during a webinar session. For
        technical reasons, this call cannot be executed from this documentation. Please
        use the curl command to execute it.
      operationId: getAttendeeQuestions
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Sessions
      - SessionKey
      - Attendees
      - RegistrantKey
      - Questions
  /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/surveys:
    get:
      summary: Get attendee survey answers
      description: Retrieve survey answers from a particular attendee during a webinar
        session. For technical reasons, this call cannot be executed from this documentation.
        Please use the curl command to execute it.
      operationId: getAttendeeSurveyAnswers
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Sessions
      - SessionKey
      - Attendees
      - RegistrantKey
      - Surveys
  /organizers/{organizerKey}/webinars/{webinarKey}/registrants:
    get:
      summary: Get registrants
      description: Retrieve registration details for all registrants of a specific
        webinar. Registrant details will not include all fields captured when creating
        the registrant. To see all data, use the API call 'Get Registrant'. Registrants
        can have one of the following states; <br>WAITING - registrant registered
        and is awaiting approval (where organizer has required approval), <br>APPROVED
        - registrant registered and is approved, and <br>DENIED - registrant registered
        and was denied.
      operationId: getAllRegistrantsForWebinar
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeyregistrants-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Registrants
    post:
      summary: Create registrant
      description: 'Register an attendee for a scheduled webinar. The response contains
        the registrantKey and join URL for the registrant. An email will be sent to
        the registrant unless the organizer turns off the confirmation email setting
        from the GoToWebinar website. Please note that you must provide all required
        fields including custom fields defined during the webinar creation. Use the
        API call ''Get registration fields'' to get a list of all fields, if they
        are required, and their possible values. At this time there are two versions
        of the ''Create Registrant'' call. The first version only accepts firstName,
        lastName, and email and ignores all other fields. If you have custom fields
        or want to capture additional information this version won''t work for you.
        The second version allows you to pass all required and optional fields, including
        custom fields defined when creating the webinar. To use the second version
        you must pass the header value ''Accept: application/vnd.citrix.g2wapi-v1.1+json''
        instead of ''Accept: application/json''. Leaving this header out results in
        the first version of the API call.'
      operationId: createRegistrant
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeyregistrants-post
      parameters:
      - in: header
        name: Accept
        description: Set to application/vnd
      - in: body
        name: body
        description: The registrant details
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: resendConfirmation
        description: Indicates whether the confirmation email should be resent when
          a registrant is re-registered
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Registrants
  /organizers/{organizerKey}/webinars/{webinarKey}/registrants/fields:
    get:
      summary: Get registration fields
      description: Retrieve required, optional registration, and custom questions
        for a specified webinar.
      operationId: getRegistrationFields
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeyregistrantsfields-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Registrants
      - Fields