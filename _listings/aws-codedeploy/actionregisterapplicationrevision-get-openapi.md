---
swagger: "2.0"
x-collection-name: AWS CodeDeploy
x-complete: 0
info:
  title: AWS CodeDeploy API Register Application Revision
  version: 1.0.0
  description: Registers with AWS CodeDeploy a revision for the specified application.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterApplicationRevision:
    get:
      summary: Register Application Revision
      description: Registers with AWS CodeDeploy a revision for the specified application.
      operationId: registerApplicationRevision
      x-api-path-slug: actionregisterapplicationrevision-get
      parameters:
      - in: query
        name: applicationName
        description: The name of an AWS CodeDeploy application associated with the
          applicable IAM user            or AWS account
        type: string
      - in: query
        name: description
        description: A comment about the revision
        type: string
      - in: query
        name: revision
        description: Information about the application revision to register, including
          type and            location
        type: string
      responses:
        200:
          description: OK
      tags:
      - Application Revisions
  /?Action=RegisterOnPremisesInstance:
    get:
      summary: Register On Premises Instance
      description: Registers an on-premises instance.
      operationId: registerOnPremisesInstance
      x-api-path-slug: actionregisteronpremisesinstance-get
      parameters:
      - in: query
        name: iamSessionArn
        description: The ARN of the IAM session to associate with the on-premises
          instance
        type: string
      - in: query
        name: iamUserArn
        description: The ARN of the IAM user to associate with the on-premises instance
        type: string
      - in: query
        name: instanceName
        description: The name of the on-premises instance to register
        type: string
      responses:
        200:
          description: OK
      tags:
      - On Premises Instances
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