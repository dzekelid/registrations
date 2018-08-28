---
swagger: "2.0"
x-collection-name: AWS Batch
x-complete: 0
info:
  title: AWS Batch API Register Job Definition
  version: 1.0.0
  description: Registers an AWS Batch job definition.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterJobDefinition:
    get:
      summary: Register Job Definition
      description: Registers an AWS Batch job definition.
      operationId: registerJobDefinition
      x-api-path-slug: actionregisterjobdefinition-get
      parameters:
      - in: query
        name: containerProperties
        description: An object with various properties specific for container-based
          jobs
        type: string
      - in: query
        name: jobDefinitionName
        description: The name of the job definition to register
        type: string
      - in: query
        name: parameters
        description: Default parameter substitution placeholders to set in the job
          definition
        type: string
      - in: query
        name: type
        description: The type of job definition
        type: string
      responses:
        200:
          description: OK
      tags:
      - Job Definitions
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