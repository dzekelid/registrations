swagger: "2.0"
x-collection-name: AWS Inspector
x-complete: 1
info:
  title: AWS Inspector API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterCrossAccountAccessRole:
    get:
      summary: Register Cross Account Access Role
      description: |-
        Registers the IAM role that Amazon Inspector uses to list your EC2 instances at the
                 start of the assessment run or when you call the.
      operationId: registerCrossAccountAccessRole
      x-api-path-slug: actionregistercrossaccountaccessrole-get
      parameters:
      - in: query
        name: roleArn
        description: The ARN of the IAM role that Amazon Inspector uses to list your
          EC2 instances during         the assessment run or when you call the PreviewAgents
          action
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cross Account Access Roles