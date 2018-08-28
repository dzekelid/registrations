---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Register Default Patch Baseline
  version: 1.0.0
  description: Defines the default patch baseline.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterDefaultPatchBaseline:
    get:
      summary: Register Default Patch Baseline
      description: Defines the default patch baseline.
      operationId: registerDefaultPatchBaseline
      x-api-path-slug: actionregisterdefaultpatchbaseline-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline that should be the default patch
          baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Default
      - Baseline
  /?Action=RegisterPatchBaselineForPatchGroup:
    get:
      summary: Register Patch Baseline For Patch Group
      description: Registers a patch baseline for a patch group.
      operationId: registerPatchBaselineForPatchGroup
      x-api-path-slug: actionregisterpatchbaselineforpatchgroup-get
      parameters:
      - in: query
        name: BaselineId
        description: The ID of the patch baseline to register the patch group with
        type: string
      - in: query
        name: PatchGroup
        description: The name of the patch group that should be registered with the
          patch baseline
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - BaselineGroup
  /?Action=RegisterTargetWithMaintenanceWindow:
    get:
      summary: Register Target With Maintenance Window
      description: Registers a target with a Maintenance Window.
      operationId: registerTargetWithMaintenanceWindow
      x-api-path-slug: actionregistertargetwithmaintenancewindow-get
      parameters:
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: OwnerInformation
        description: User-provided value that will be included in any CloudWatch events
          raised while running   tasks for these targets in this Maintenance Window
        type: string
      - in: query
        name: ResourceType
        description: The type of target being registered with the Maintenance Window
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags)
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window the target should be registered
          with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - TargetMaintenance
      - Window
  /?Action=RegisterTaskWithMaintenanceWindow:
    get:
      summary: Register Task With Maintenance Window
      description: Adds a new task to a Maintenance Window.
      operationId: registerTaskWithMaintenanceWindow
      x-api-path-slug: actionregistertaskwithmaintenancewindow-get
      parameters:
      - in: query
        name: ClientToken
        description: User-provided idempotency token
        type: string
      - in: query
        name: LoggingInfo
        description: A structure containing information about an Amazon S3 bucket
          to write instance-level logs to
        type: string
      - in: query
        name: MaxConcurrency
        description: The maximum number of targets this task can be run for in parallel
        type: string
      - in: query
        name: MaxErrors
        description: The maximum number of errors allowed before this task stops being
          scheduled
        type: string
      - in: query
        name: Priority
        description: The priority of the task in the Maintenance Window, the lower
          the number the higher the   priority
        type: string
      - in: query
        name: ServiceRoleArn
        description: The role that should be assumed when executing the task
        type: string
      - in: query
        name: Targets
        description: The targets (either instances or tags)
        type: string
      - in: query
        name: TaskArn
        description: The ARN of the task to execute
        type: string
      - in: query
        name: TaskParameters
        description: The parameters that should be passed to the task when it is executed
        type: string
      - in: query
        name: TaskType
        description: The type of task being registered
        type: string
      - in: query
        name: WindowId
        description: The id of the Maintenance Window the task should be added to
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - TaskMaintenance
      - Window
  /?Action=CreateActivation:
    get:
      summary: Create Activation
      description: |-
        Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage
           these resources using Run Command.
      operationId: createActivation
      x-api-path-slug: actioncreateactivation-get
      parameters:
      - in: query
        name: DefaultInstanceName
        description: The name of the registered, managed instance as it will appear
          in the Amazon EC2 console or   when you use the AWS command line tools to
          list EC2 resources
        type: string
      - in: query
        name: Description
        description: A user-defined description of the resource that you want to register
          with Amazon EC2
        type: string
      - in: query
        name: ExpirationDate
        description: The date by which this activation request should expire
        type: string
      - in: query
        name: IamRole
        description: The Amazon Identity and Access Management (IAM) role that you
          want to assign to the   managed instance
        type: string
      - in: query
        name: RegistrationLimit
        description: Specify the maximum number of managed instances you want to register
        type: string
      responses:
        200:
          description: OK
      tags:
      - Activation
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