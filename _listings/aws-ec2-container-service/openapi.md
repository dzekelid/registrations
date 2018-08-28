swagger: "2.0"
x-collection-name: AWS EC2 Container Service
x-complete: 1
info:
  title: AWS EC2 Container Service API
  version: 1.0.0
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
  /?Action=RegisterTaskDefinition:
    get:
      summary: Register Task Definition
      description: |-
        Registers a new task definition from the supplied family and
                        containerDefinitions.
      operationId: registerTaskDefinition
      x-api-path-slug: actionregistertaskdefinition-get
      parameters:
      - in: query
        name: containerDefinitions
        description: A list of container definitions in JSON format that describe
          the different            containers that make up your task
        type: string
      - in: query
        name: family
        description: You must specify a family for a task definition, which allows
          you to            track multiple versions of the same task definition
        type: string
      - in: query
        name: networkMode
        description: The Docker networking mode to use for the containers in the task
        type: string
      - in: query
        name: placementConstraints
        description: An array of placement constraint objects to use for the task
        type: string
      - in: query
        name: taskRoleArn
        description: The short name or full Amazon Resource Name (ARN) of the IAM
          role that containers in this task can            assume
        type: string
      - in: query
        name: volumes
        description: A list of volume definitions in JSON format that containers in
          your task may            use
        type: string
      responses:
        200:
          description: OK
      tags:
      - Task Definitions