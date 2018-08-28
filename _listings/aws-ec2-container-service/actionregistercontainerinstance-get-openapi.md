---
swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 0
info:
  title: Amazon EC2 Container Service API Register Container Instance
  version: 1.0.0
  description: Deregisters an Amazon ECS container instance from the specified cluster.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterContainerInstance:
    get:
      summary: Register Container Instance
      description: Deregisters an Amazon ECS container instance from the specified
        cluster.
      operationId: registerContainerInstance
      x-api-path-slug: actionregistercontainerinstance-get
      responses:
        200:
          description: OK
      tags:
      - Containers
      - Instances
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