swagger: "2.0"
x-collection-name: AWS Elastic Load Balancing
x-complete: 1
info:
  title: AWS Elastic Load Balancing API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterTargets:
    get:
      summary: Register Targets
      description: Registers the specified targets with the specified target group.
      operationId: registerTargets
      x-api-path-slug: actionregistertargets-get
      parameters:
      - in: query
        name: TargetGroupArn
        description: The Amazon Resource Name (ARN) of the target group
        type: string
      - in: query
        name: Targets.member.N
        description: The targets
        type: string
      responses:
        200:
          description: OK
      tags:
      - Targets