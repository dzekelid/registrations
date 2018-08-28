swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterEcsCluster:
    get:
      summary: Register Ecs Cluster
      description: Registers a specified Amazon ECS cluster with a stack.
      operationId: registerEcsCluster
      x-api-path-slug: actionregisterecscluster-get
      parameters:
      - in: query
        name: EcsClusterArn
        description: The clusters ARN
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Ecs
      - Cluster
  /?Action=RegisterElasticIp:
    get:
      summary: Register Elastic Ip
      description: Registers an Elastic IP address with a specified stack.
      operationId: registerElasticIp
      x-api-path-slug: actionregisterelasticip-get
      parameters:
      - in: query
        name: ElasticIp
        description: The Elastic IP address
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Elastic
      - Ip
  /?Action=RegisterInstance:
    get:
      summary: Register Instance
      description: Registers instances that were created outside of AWS OpsWorks Stacks
        with a specified stack.
      operationId: registerInstance
      x-api-path-slug: actionregisterinstance-get
      parameters:
      - in: query
        name: Hostname
        description: The instances hostname
        type: string
      - in: query
        name: InstanceIdentity
        description: An InstanceIdentity object that contains the instances identity
        type: string
      - in: query
        name: PrivateIp
        description: The instances private IP address
        type: string
      - in: query
        name: PublicIp
        description: The instances public IP address
        type: string
      - in: query
        name: RsaPublicKey
        description: The instances public RSA key
        type: string
      - in: query
        name: RsaPublicKeyFingerprint
        description: The instances public RSA key fingerprint
        type: string
      - in: query
        name: StackId
        description: The ID of the stack that the instance is to be registered with
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Instance
  /?Action=RegisterRdsDbInstance:
    get:
      summary: Register Rds Db Instance
      description: Registers an Amazon RDS instance with a stack.
      operationId: registerRdsDbInstance
      x-api-path-slug: actionregisterrdsdbinstance-get
      parameters:
      - in: query
        name: DbPassword
        description: The database password
        type: string
      - in: query
        name: DbUser
        description: The databases master user name
        type: string
      - in: query
        name: RdsDbInstanceArn
        description: The Amazon RDS instances ARN
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Rds
      - Db
      - Instance
  /?Action=RegisterVolume:
    get:
      summary: Register Volume
      description: Registers an Amazon EBS volume with a specified stack.
      operationId: registerVolume
      x-api-path-slug: actionregistervolume-get
      parameters:
      - in: query
        name: Ec2VolumeId
        description: The Amazon EBS volume ID
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Register
      - Volume