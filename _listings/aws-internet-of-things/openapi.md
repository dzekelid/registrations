swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 1
info:
  title: AWS Internet of Things API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteRegistrationCode:
    get:
      summary: Delete Registration Code
      description: Deletes a CA certificate registration code.
      operationId: deleteRegistrationCode
      x-api-path-slug: actiondeleteregistrationcode-get
      responses:
        200:
          description: OK
      tags:
      - Registration Codes
  /?Action=GetRegistrationCode:
    get:
      summary: Get Registration Code
      description: Gets a registration code used to register a CA certificate with
        AWS IoT.
      operationId: getRegistrationCode
      x-api-path-slug: actiongetregistrationcode-get
      parameters:
      - in: query
        name: registrationCode
        description: The CA certificate registration code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Registration Codes
  /?Action=RegisterCACertificate:
    get:
      summary: Register C A Certificate
      description: Registers a CA certificate with AWS IoT.
      operationId: registerCACertificate
      x-api-path-slug: actionregistercacertificate-get
      parameters:
      - in: query
        name: allowAutoRegistration
        description: Allows this CA certificate to be used for auto registration of
          device certificates
        type: string
      - in: query
        name: caCertificate
        description: The CA certificate
        type: string
      - in: query
        name: setAsActive
        description: A boolean value that specifies if the CA certificate is set to
          active
        type: string
      - in: query
        name: verificationCertificate
        description: The private key verification certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
  /?Action=RegisterCertificate:
    get:
      summary: Register Certificate
      description: Registers a device certificate with AWS IoT.
      operationId: registerCertificate
      x-api-path-slug: actionregistercertificate-get
      parameters:
      - in: query
        name: caCertificatePem
        description: The CA certificate used to sign the device certificate being
          registered
        type: string
      - in: query
        name: certificatePem
        description: The certificate data, in PEM format
        type: string
      - in: query
        name: setAsActive
        description: A boolean value that specifies if the CA certificate is set to
          active
        type: string
      - in: query
        name: status
        description: The status of the register certificate request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates