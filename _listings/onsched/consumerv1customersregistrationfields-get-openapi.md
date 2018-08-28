---
swagger: "2.0"
x-collection-name: OnSched
x-complete: 0
info:
  title: OnSched Returns a list of lead questions
  description: "This end point returns your Customer Registration fields.\r\n\r\nCustomer
    custom fields are different than Appointment custom fields. Appointment custom
    fields are\r\nstored with each appointment. They are used when the information
    collected during the booking is specific\r\nto a particular visit, where as Customer
    custom fields are stored with the customer profile."
  termsOfService: None
  contact:
    name: OnSched.com
    url: https://onsched.com
    email: info@onsched.com
  version: 1.0.0
host: api.onsched.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /consumer/v1/customers/registrationfields:
    get:
      summary: Returns a list of lead questions
      description: "This end point returns your Customer Registration fields.\r\n\r\nCustomer
        custom fields are different than Appointment custom fields. Appointment custom
        fields are\r\nstored with each appointment. They are used when the information
        collected during the booking is specific\r\nto a particular visit, where as
        Customer custom fields are stored with the customer profile."
      operationId: ConsumerV1CustomersRegistrationfieldsGet
      x-api-path-slug: consumerv1customersregistrationfields-get
      parameters:
      - in: query
        name: locationId
        description: The id of the business location
      responses:
        200:
          description: OK
      tags:
      - Customers
      - Registrationfields
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