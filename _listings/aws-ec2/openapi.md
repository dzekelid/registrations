swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 1
info:
  title: AWS EC2 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterImage:
    get:
      summary: Register Image
      description: Registers an AMI.
      operationId: registerimage
      x-api-path-slug: actionregisterimage-get
      parameters:
      - in: query
        name: Attribute
        description: The attribute to reset (currently you can only reset the launch
          permission attribute)
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: ImageId
        description: The ID of the AMI
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Image