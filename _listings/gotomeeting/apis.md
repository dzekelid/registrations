---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Registrations
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Get Training Registrants
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
  description: 'Retrieves details on all registrants for a specific training. Registrants
    can be:<br>WAITING - registrant registered and is awaiting approval (where organizer
    has required approval)<br>APPROVED - registrant registered and is approved<br>DENIED
    - registrant registered and was not approved.<br><br>IMPORTANT: The registrant
    data caches are typically updated immediately and the data will be returned in
    the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-get-openapi.md
- name: Go To Training - Register for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
  description: 'Registers one person, identified by a unique email address, for a
    training. Approval is automatic unless payment or approval is required. The response
    contains the Confirmation page URL and Join URL for the registrant. NOTE: If some
    registrants do not receive a confirmation email, the emails could be getting blocked
    by their email server due to spam filtering or a grey-listing setting.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-post-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Update Training Registration Settings
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
  description: An API request to automatically enable or disable web registrations
    and confirmation emails to registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrationsettings-put-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Get Training Registrants
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
  description: 'Retrieves details on all registrants for a specific training. Registrants
    can be:<br>WAITING - registrant registered and is awaiting approval (where organizer
    has required approval)<br>APPROVED - registrant registered and is approved<br>DENIED
    - registrant registered and was not approved.<br><br>IMPORTANT: The registrant
    data caches are typically updated immediately and the data will be returned in
    the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-get-openapi.md
- name: Go To Training - Register for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
  description: 'Registers one person, identified by a unique email address, for a
    training. Approval is automatic unless payment or approval is required. The response
    contains the Confirmation page URL and Join URL for the registrant. NOTE: If some
    registrants do not receive a confirmation email, the emails could be getting blocked
    by their email server due to spam filtering or a grey-listing setting.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-post-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Update Training Registration Settings
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
  description: An API request to automatically enable or disable web registrations
    and confirmation emails to registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrationsettings-put-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Get Registrant
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get
  description: 'Retrieves details for specific registrant in a specific training.
    Registrants can be:<br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval)<br>APPROVED - registrant registered and
    is approved<br>DENIED - registrant registered and was not approved.<br><br>IMPORTANT:
    The registrant data caches are typically updated immediately and the data will
    be returned in the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Training - Cancel Registration
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete
  description: This call cancels a registration in a scheduled training for a specific
    registrant. If the registrant has paid for the training, a cancellation cannot
    be completed with this method; it must be completed on the external admin site.
    No notification is sent to the registrant or the organizer by default. The registrant
    can re-register if needed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Training - Register for Training
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-post
  description: 'Registers one person, identified by a unique email address, for a
    training. Approval is automatic unless payment or approval is required. The response
    contains the Confirmation page URL and Join URL for the registrant. NOTE: If some
    registrants do not receive a confirmation email, the emails could be getting blocked
    by their email server due to spam filtering or a grey-listing setting.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-post-openapi.md
- name: Go To Training - Get Training Registrants
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrants-get
  description: 'Retrieves details on all registrants for a specific training. Registrants
    can be:<br>WAITING - registrant registered and is awaiting approval (where organizer
    has required approval)<br>APPROVED - registrant registered and is approved<br>DENIED
    - registrant registered and was not approved.<br><br>IMPORTANT: The registrant
    data caches are typically updated immediately and the data will be returned in
    the response. However, the update can take as long as two hours.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrants-get-openapi.md
- name: Go To Training - Update Training Registration Settings
  x-api-slug: organizersorganizerkeytrainingstrainingkeyregistrationsettings-put
  description: An API request to automatically enable or disable web registrations
    and confirmation emails to registrants.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeytrainingstrainingkeyregistrationsettings-put-openapi.md
- name: Go To Webinar - Delete registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
  description: Removes a webinar registrant from current registrations for the specified
    webinar. The webinar must be a scheduled, future webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Webinar - Get registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get
  description: Retrieve registration details for a specific registrant.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Webinar - Get attendee
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
  description: Retrieve registration details for a particular attendee of a specific
    webinar session. For technical reasons, this call cannot be executed from this
    documentation. Please use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-openapi.md
- name: Go To Webinar - Get attendee poll answers
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
  description: Get poll answers from a particular attendee of a specific webinar session.
    For technical reasons, this call cannot be executed from this documentation. Please
    use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-openapi.md
- name: Go To Webinar - Get attendee questions
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
  description: Get questions asked by an attendee during a webinar session. For technical
    reasons, this call cannot be executed from this documentation. Please use the
    curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-openapi.md
- name: Go To Webinar - Get attendee survey answers
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
  description: Retrieve survey answers from a particular attendee during a webinar
    session. For technical reasons, this call cannot be executed from this documentation.
    Please use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-openapi.md
- name: Go To Webinar - Get registrants
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrants-get
  description: Retrieve registration details for all registrants of a specific webinar.
    Registrant details will not include all fields captured when creating the registrant.
    To see all data, use the API call 'Get Registrant'. Registrants can have one of
    the following states; <br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval), <br>APPROVED - registrant registered
    and is approved, and <br>DENIED - registrant registered and was denied.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrants-get-openapi.md
- name: Go To Webinar - Create registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrants-post
  description: 'Register an attendee for a scheduled webinar. The response contains
    the registrantKey and join URL for the registrant. An email will be sent to the
    registrant unless the organizer turns off the confirmation email setting from
    the GoToWebinar website. Please note that you must provide all required fields
    including custom fields defined during the webinar creation. Use the API call
    ''Get registration fields'' to get a list of all fields, if they are required,
    and their possible values. At this time there are two versions of the ''Create
    Registrant'' call. The first version only accepts firstName, lastName, and email
    and ignores all other fields. If you have custom fields or want to capture additional
    information this version won''t work for you. The second version allows you to
    pass all required and optional fields, including custom fields defined when creating
    the webinar. To use the second version you must pass the header value ''Accept:
    application/vnd.citrix.g2wapi-v1.1+json'' instead of ''Accept: application/json''.
    Leaving this header out results in the first version of the API call.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrants-post-openapi.md
- name: Go To Webinar - Get registration fields
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsfields-get
  description: Retrieve required, optional registration, and custom questions for
    a specified webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsfields-get-openapi.md
- name: Go To Webinar - Delete registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
  description: Removes a webinar registrant from current registrations for the specified
    webinar. The webinar must be a scheduled, future webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Webinar - Get registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get
  description: Retrieve registration details for a specific registrant.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Webinar - Delete registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
  description: Removes a webinar registrant from current registrations for the specified
    webinar. The webinar must be a scheduled, future webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Webinar - Get registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get
  description: Retrieve registration details for a specific registrant.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Webinar - Get attendee
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
  description: Retrieve registration details for a particular attendee of a specific
    webinar session. For technical reasons, this call cannot be executed from this
    documentation. Please use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-openapi.md
- name: Go To Webinar - Get attendee poll answers
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
  description: Get poll answers from a particular attendee of a specific webinar session.
    For technical reasons, this call cannot be executed from this documentation. Please
    use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-openapi.md
- name: Go To Webinar - Get attendee questions
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
  description: Get questions asked by an attendee during a webinar session. For technical
    reasons, this call cannot be executed from this documentation. Please use the
    curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-openapi.md
- name: Go To Webinar - Get attendee survey answers
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
  description: Retrieve survey answers from a particular attendee during a webinar
    session. For technical reasons, this call cannot be executed from this documentation.
    Please use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-openapi.md
- name: Go To Webinar - Get registrants
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrants-get
  description: Retrieve registration details for all registrants of a specific webinar.
    Registrant details will not include all fields captured when creating the registrant.
    To see all data, use the API call 'Get Registrant'. Registrants can have one of
    the following states; <br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval), <br>APPROVED - registrant registered
    and is approved, and <br>DENIED - registrant registered and was denied.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrants-get-openapi.md
- name: Go To Webinar - Create registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrants-post
  description: 'Register an attendee for a scheduled webinar. The response contains
    the registrantKey and join URL for the registrant. An email will be sent to the
    registrant unless the organizer turns off the confirmation email setting from
    the GoToWebinar website. Please note that you must provide all required fields
    including custom fields defined during the webinar creation. Use the API call
    ''Get registration fields'' to get a list of all fields, if they are required,
    and their possible values. At this time there are two versions of the ''Create
    Registrant'' call. The first version only accepts firstName, lastName, and email
    and ignores all other fields. If you have custom fields or want to capture additional
    information this version won''t work for you. The second version allows you to
    pass all required and optional fields, including custom fields defined when creating
    the webinar. To use the second version you must pass the header value ''Accept:
    application/vnd.citrix.g2wapi-v1.1+json'' instead of ''Accept: application/json''.
    Leaving this header out results in the first version of the API call.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrants-post-openapi.md
- name: Go To Webinar - Get registration fields
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsfields-get
  description: Retrieve required, optional registration, and custom questions for
    a specified webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsfields-get-openapi.md
- name: Go To Webinar - Delete registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
  description: Removes a webinar registrant from current registrations for the specified
    webinar. The webinar must be a scheduled, future webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Webinar - Get registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get
  description: Retrieve registration details for a specific registrant.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Webinar - Get attendee survey answers
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
  description: Retrieve survey answers from a particular attendee during a webinar
    session. For technical reasons, this call cannot be executed from this documentation.
    Please use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-openapi.md
- name: Go To Webinar - Get attendee questions
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
  description: Get questions asked by an attendee during a webinar session. For technical
    reasons, this call cannot be executed from this documentation. Please use the
    curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-openapi.md
- name: Go To Webinar - Get attendee poll answers
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
  description: Get poll answers from a particular attendee of a specific webinar session.
    For technical reasons, this call cannot be executed from this documentation. Please
    use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-openapi.md
- name: Go To Webinar - Get attendee
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
  description: Retrieve registration details for a particular attendee of a specific
    webinar session. For technical reasons, this call cannot be executed from this
    documentation. Please use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-openapi.md
- name: Go To Webinar - Get registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get
  description: Retrieve registration details for a specific registrant.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Webinar - Delete registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
  description: Removes a webinar registrant from current registrations for the specified
    webinar. The webinar must be a scheduled, future webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Webinar - Get registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get
  description: Retrieve registration details for a specific registrant.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-get-openapi.md
- name: Go To Webinar - Delete registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete
  description: Removes a webinar registrant from current registrations for the specified
    webinar. The webinar must be a scheduled, future webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsregistrantkey-delete-openapi.md
- name: Go To Webinar - Get registration fields
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrantsfields-get
  description: Retrieve required, optional registration, and custom questions for
    a specified webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrantsfields-get-openapi.md
- name: Go To Webinar - Create registrant
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrants-post
  description: 'Register an attendee for a scheduled webinar. The response contains
    the registrantKey and join URL for the registrant. An email will be sent to the
    registrant unless the organizer turns off the confirmation email setting from
    the GoToWebinar website. Please note that you must provide all required fields
    including custom fields defined during the webinar creation. Use the API call
    ''Get registration fields'' to get a list of all fields, if they are required,
    and their possible values. At this time there are two versions of the ''Create
    Registrant'' call. The first version only accepts firstName, lastName, and email
    and ignores all other fields. If you have custom fields or want to capture additional
    information this version won''t work for you. The second version allows you to
    pass all required and optional fields, including custom fields defined when creating
    the webinar. To use the second version you must pass the header value ''Accept:
    application/vnd.citrix.g2wapi-v1.1+json'' instead of ''Accept: application/json''.
    Leaving this header out results in the first version of the API call.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrants-post-openapi.md
- name: Go To Webinar - Get registrants
  x-api-slug: organizersorganizerkeywebinarswebinarkeyregistrants-get
  description: Retrieve registration details for all registrants of a specific webinar.
    Registrant details will not include all fields captured when creating the registrant.
    To see all data, use the API call 'Get Registrant'. Registrants can have one of
    the following states; <br>WAITING - registrant registered and is awaiting approval
    (where organizer has required approval), <br>APPROVED - registrant registered
    and is approved, and <br>DENIED - registrant registered and was denied.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/registrations/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyregistrants-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.url.shortener.api.gallery.streamdata.io
- type: x-api-stack
  url: http://gotomeeting.stack.network
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---