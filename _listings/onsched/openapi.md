swagger: "2.0"
x-collection-name: OnSched
x-complete: 1
info:
  title: OnSched API
  description: build-secure-and-scalable-custom-apps-for-online-booking--our-flexible-api-provides-many-options-for-availability-and-booking--take-the-api-for-a-test-drive--just-click-on-the-authorize-button-above-and-authenticate---you-can-access-our-demo-company-profile-if-you-are-not-a-customer-or-your-own-profile-by-using-your-assigned-clientid-and-secret---------------------
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