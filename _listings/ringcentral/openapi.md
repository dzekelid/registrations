swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/client-info/sip-provision:
    post:
      summary: Register SIP Device
      description: "Creates SIP registration of a device/application (WebPhone, Mobile,
        softphone)\nApp Permission\nVoipCalling\nUsage Plan Group\nHeavy\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [sipInfo.transport] value is invalid\n\n\n400\nSPR-114\nDevice id length [40]
        is greater than allowed [38]\n\n\n400\nSPR-118\nParameter [device.id]=@1qwbc)yppa!
        is not a number\n\n\n400\nSPR-129\nNot allowed to register with incompatible
        protocol list [WS, TCP]\n\n\n400\nSPR-130\ndevice is not allowed for WebRTC.\n\n\n403\nBIL-103\nFeature
        [WebPhone] is not available for current account\n\n\n403\nCMN-401\nIn order
        to call this API endpoint, application needs to have [VoipCalling] permission\n\n\n403\nCMN-402\nAdministrator
        permission required\n\n\n403\nSPR-112\nClient edition is not compatible with
        current Brand\n\n\n403\nSPR-122\nApplication version is not set in \"User-Agent\"
        header or not parseable"
      operationId: createSipRegistration
      x-api-path-slug: restapiv1-0clientinfosipprovision-post
      parameters:
      - in: body
        name: body
        description: JSON body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Register
      - SIP
      - Device