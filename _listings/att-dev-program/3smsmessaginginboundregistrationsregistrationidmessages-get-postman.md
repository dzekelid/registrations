{
  "info": {
    "name": "AT&T API Get SMS Inbound Registrations Registrationid Messages",
    "_postman_id": "9d44e5e5-db05-42c4-9a2e-34ac24215580",
    "description": "/3/smsmessaging/inbound/registrations/{registrationId}/messages",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Devicecapabilities",
      "item": [
        {
          "id": "2dca771a-4be9-4dae-b9c7-32a7b4e2c800",
          "name": "1devicecapabilitiesacrauthorizationcapabilities",
          "request": {
            "url": "http://api.att.com/1/devicecapabilities/acr:authorization/capabilities",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/1/devicecapabilities/acr:authorization/capabilities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6bbcc25-b5e2-46bf-8bfa-f15c916b268b"
            }
          ]
        }
      ]
    },
    {
      "name": "Messaging",
      "item": [
        {
          "id": "c5d94ccd-dd8b-4850-9b6c-0555a07911e8",
          "name": "3messagingoutboundsenderaddressrequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/messaging/outbound/:senderAddress/requests"
              ],
              "variable": [
                {
                  "id": "senderAddress",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/3/messaging/outbound/{senderAddress}/requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a09b064-e61d-4e30-b5fd-d8ae39e1a843"
            }
          ]
        },
        {
          "id": "c90dcb34-975a-403e-bd6e-41c8e29b71da",
          "name": "3messagingoutboundsenderaddressrequestiddeliveryinfos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/messaging/outbound/:senderAddress/:requestId/deliveryInfos"
              ],
              "variable": [
                {
                  "id": "requestId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "senderAddress",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/3/messaging/outbound/{senderAddress}/{requestId}/deliveryInfos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2129499-3210-461b-809a-3547c8881e8c"
            }
          ]
        }
      ]
    },
    {
      "name": "Smsmessaging",
      "item": [
        {
          "id": "198cd23e-9283-434f-8b07-1f4938766342",
          "name": "3smsmessaginginboundregistrationsregistrationidmessages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/smsmessaging/inbound/registrations/:registrationId/messages"
              ],
              "variable": [
                {
                  "id": "registrationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/3/smsmessaging/inbound/registrations/{registrationId}/messages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6ddef7d-a5b6-4e6b-9f8b-7a7445579d6a"
            }
          ]
        }
      ]
    }
  ]
}