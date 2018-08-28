swagger: "2.0"
x-collection-name: AT&T Dev Program
x-complete: 1
info:
  title: AT&T Dev Program Merged API
  version: 1.0.0
host: api.att.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /3/smsmessaging/inbound/registrations/{registrationId}/messages:
    get:
      summary: Get SMS Inbound Registrations Registrationid Messages
      description: /3/smsmessaging/inbound/registrations/{registrationId}/messages
      operationId: 3smsmessaginginboundregistrationsregistrationidmessages
      x-api-path-slug: 3smsmessaginginboundregistrationsregistrationidmessages-get
      parameters:
      - in: path
        name: registrationId
      responses:
        200:
          description: OK
      tags:
      - Smsmessaging
      - Inbound
      - Registrations
      - RegistrationId
      - Messages
  /sms/v3/messaging/inbox/{RegistrationID}:
    get:
      summary: Get SMS Messaging Inbox Registration
      description: /sms/v3/messaging/inbox/{RegistrationID}
      operationId: smsv3messaginginboxregistrationid
      x-api-path-slug: smsv3messaginginboxregistrationid-get
      parameters:
      - in: path
        name: RegistrationID
      responses:
        200:
          description: OK
      tags:
      - Sms
      - VMessaging
      - Inbox
      - RegistrationID