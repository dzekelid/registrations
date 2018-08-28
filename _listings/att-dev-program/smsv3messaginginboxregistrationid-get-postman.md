{
  "info": {
    "name": "AT&T API Get SMS Messaging Inbox Registration",
    "_postman_id": "6d85a7a4-3217-40f3-a955-9cf344275dcc",
    "description": "/sms/v3/messaging/inbox/{RegistrationID}",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Devicecapabilities",
      "item": [
        {
          "id": "11af56ea-35f6-48b6-9105-86be4ec033bd",
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
              "id": "abd7d2c3-5c31-475e-8ea4-4f01145324ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Messaging",
      "item": [
        {
          "id": "3a71e153-f661-4c03-8e9a-cb8b90008bb4",
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
              "id": "bb51efec-2140-48ac-b6d7-e296417216bd"
            }
          ]
        },
        {
          "id": "d821f09e-92b6-454d-bd81-b37897d57de1",
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
              "id": "29e80129-58ba-4ffd-9d4b-373976e234de"
            }
          ]
        }
      ]
    },
    {
      "name": "Smsmessaging",
      "item": [
        {
          "id": "c7b18db2-4db2-41f4-af8c-6ede24986342",
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
              "id": "bb6c0a9a-8d1f-4769-9add-25ea200f4ebd"
            }
          ]
        },
        {
          "id": "b5f2cd00-1774-4587-b409-210d2f60a153",
          "name": "3smsmessagingoutboundrequestssenderaddressrequestiddeliveryinfos",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/smsmessaging/outbound/requests/:senderAddress/:requestId/deliveryInfos"
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
            "description": "/3/smsmessaging/outbound/requests/{senderAddress}/{requestId}/deliveryInfos"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "676df4a7-8e41-472d-a8f3-419de1522d4b"
            }
          ]
        },
        {
          "id": "1320ab1f-2b09-4015-a6b3-0efad3a3e24a",
          "name": "3smsmessagingoutboundsenderaddressrequests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "3/smsmessaging/outbound/:senderAddress/requests"
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
            "description": "/3/smsmessaging/outbound/{senderAddress}/requests"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "76e926e4-4fb8-488b-a74c-4139dcfefaaa"
            }
          ]
        }
      ]
    },
    {
      "name": "Mms",
      "item": [
        {
          "id": "1ccd791a-b784-419c-9964-ee5e9695c845",
          "name": "mmsv3messagingoutbox",
          "request": {
            "url": "http://api.att.com/mms/v3/messaging/outbox",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/mms/v3/messaging/outbox"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb4cf317-0650-4d95-bb5f-adc6507109dd"
            }
          ]
        },
        {
          "id": "02057a0a-5de0-4836-b83e-a2554c20fa69",
          "name": "mmsv3messagingoutboxmessageid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "mms/v3/messaging/outbox/:messageId"
              ],
              "variable": [
                {
                  "id": "messageId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/mms/v3/messaging/outbox/{messageId}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f251bd5b-b047-4a27-9409-2b5eb07dcec6"
            }
          ]
        }
      ]
    },
    {
      "name": "MyMessages",
      "item": [
        {
          "id": "ce7faa4e-ca0f-42bb-a805-662e28a4301c",
          "name": "mymessagesv2delta",
          "request": {
            "url": "http://api.att.com/myMessages/v2/delta",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/delta"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81ae61c1-d4e0-402a-adbf-6f4315e76f40"
            }
          ]
        },
        {
          "id": "27da31d1-ec7d-4e18-9702-67dd684072ff",
          "name": "mymessagesv2messages",
          "request": {
            "url": "http://api.att.com/myMessages/v2/messages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/messages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae57039b-bdf1-4b61-ae5f-6ca5c02e99d2"
            }
          ]
        },
        {
          "id": "4f6a67d3-f4b6-48a6-a321-cc0ae3f1017f",
          "name": "mymessagesv2messages",
          "request": {
            "url": "http://api.att.com/myMessages/v2/messages",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/messages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9608c47-aecb-4137-88b5-6ce2107b81b1"
            }
          ]
        },
        {
          "id": "9430352e-ca06-472c-a69b-5b1eb1a21c92",
          "name": "mymessagesv2messages",
          "request": {
            "url": "http://api.att.com/myMessages/v2/messages",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/messages"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5fbb940-2cc7-43f6-8994-7d722cb0b523"
            }
          ]
        },
        {
          "id": "3658684d-02a6-40c7-848f-e64e46c46949",
          "name": "mymessagesv2messagesindex",
          "request": {
            "url": "http://api.att.com/myMessages/v2/messages/index",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/messages/index"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de0423a2-f525-4fee-9584-90cf4761af28"
            }
          ]
        },
        {
          "id": "bee34981-04ab-4405-8839-94796f7df17a",
          "name": "mymessagesv2messagesindexinfo",
          "request": {
            "url": "http://api.att.com/myMessages/v2/messages/index/info",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/messages/index/info"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1579f1b-d4bb-4ff6-94d6-d6e2bc3e15f9"
            }
          ]
        },
        {
          "id": "0b1cb692-837a-424f-a5c7-73b751604e68",
          "name": "mymessagesv2messagesmessageid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "myMessages/v2/messages/:messageId"
              ],
              "variable": [
                {
                  "id": "messageId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/messages/{messageId}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "26e0fc14-4081-4250-b29a-68779b73dfec"
            }
          ]
        },
        {
          "id": "2861dc2e-caf3-4ef2-8732-b7a496f3fd7d",
          "name": "mymessagesv2messagesmessageid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "myMessages/v2/messages/:messageId"
              ],
              "variable": [
                {
                  "id": "messageId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/messages/{messageId}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b06370e-52f1-40f7-99e8-440747d7c821"
            }
          ]
        },
        {
          "id": "af25ff4e-6156-484c-8689-d932f8558b83",
          "name": "mymessagesv2messagesmessageidpartspartid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "myMessages/v2/messages/:messageId/parts/:partId"
              ],
              "variable": [
                {
                  "id": "messageId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "partId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/messages/{messageId}/parts/{partId}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9ae8891-dec4-4258-a8f5-973182073776"
            }
          ]
        },
        {
          "id": "ef88e81e-8764-43fb-84da-9ce42babb7c0",
          "name": "mymessagesv2notificationconnectiondetails",
          "request": {
            "url": "http://api.att.com/myMessages/v2/notificationConnectionDetails",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/myMessages/v2/notificationConnectionDetails"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93b73489-e7d4-4733-8e1c-091920103e69"
            }
          ]
        }
      ]
    },
    {
      "name": "Rest",
      "item": [
        {
          "id": "ef3fce32-ecc6-45c4-a2ac-fc4e232cae12",
          "name": "rest1ads",
          "request": {
            "url": "http://api.att.com/rest/1/ads",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/rest/1/ads"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42e9cf35-e90e-44dc-860e-b15796faea0e"
            }
          ]
        },
        {
          "id": "dd52980d-5f8b-4668-883d-7fee4b38a9ca",
          "name": "rest2devicesinfo",
          "request": {
            "url": "http://api.att.com/rest/2/Devices/Info",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/rest/2/Devices/Info"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f70673e3-af9c-453b-a4d1-3d641400fbc1"
            }
          ]
        }
      ]
    },
    {
      "name": "Sms",
      "item": [
        {
          "id": "974afd01-a645-44c3-b6a9-a776e9718cd0",
          "name": "smsv3messaginginboxregistrationid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.att.com",
              "path": [
                "sms/v3/messaging/inbox/:RegistrationID"
              ],
              "variable": [
                {
                  "id": "RegistrationID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/sms/v3/messaging/inbox/{RegistrationID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c511cdab-cf56-4dc5-a380-6e40545f6777"
            }
          ]
        }
      ]
    }
  ]
}