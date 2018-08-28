{
  "info": {
    "name": "Constant Contact List Registrants",
    "_postman_id": "c78ab56d-13f3-4333-aff6-073897b46fcf",
    "description": "List Registrants",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "12fcadc6-750d-4c37-990b-004769f6dc68",
          "name": "list-activities",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/activities"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Activities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1210c618-074e-48be-ab72-a60fd7f0458c"
            }
          ]
        },
        {
          "id": "4b9d2b54-c73e-4894-a560-5a4d52a9b177",
          "name": "list-campaigns",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/campaigns"
              ],
              "query": [
                {
                  "key": "refresh",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Campaigns"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95f0a312-63ef-4389-96b3-98a12b62b0a7"
            }
          ]
        },
        {
          "id": "d1dc6983-98a2-437b-b043-8d152ef142ec",
          "name": "list-contacts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts"
              ],
              "query": [
                {
                  "key": "listid",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "updatedsince",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Contacts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f13820e9-3c29-4d44-9d33-f81466e14372"
            }
          ]
        },
        {
          "id": "293710c1-c04c-4f9c-8721-79084c081b59",
          "name": "list-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/events"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "727c0d9f-d651-4757-9d41-c7090d87ae9b"
            }
          ]
        },
        {
          "id": "f7b8900f-60a9-4d9d-9362-817bb7127ebb",
          "name": "list-registrants",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/events/:event-id/registrants"
              ],
              "variable": [
                {
                  "id": "event-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List Registrants"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3660b562-6d39-4d8e-abb1-1177b0b5c9cb"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "c859a6dc-d5ff-4ed6-ba8d-193fc3c3f247",
          "name": "add-activity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/activities"
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add Activity"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed56c632-d970-415d-88b3-3f98537011b7"
            }
          ]
        },
        {
          "id": "fe21dacc-28cb-4f55-8f2f-46f1a2a98899",
          "name": "get-activity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/activities/:activity-id"
              ],
              "variable": [
                {
                  "id": "activity-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Activity"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0647134d-38c8-42ca-bd14-9f67cace2434"
            }
          ]
        }
      ]
    },
    {
      "name": "Campaign",
      "item": [
        {
          "id": "49ad916a-b358-42e1-83a7-9aad7b7ceac9",
          "name": "add-campaign",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/campaigns"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add Campaign"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e726add1-0501-4c37-9196-6fec22288548"
            }
          ]
        },
        {
          "id": "fa6cbd70-55ff-40c2-8844-37ecfc8e49ad",
          "name": "get-campaign",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/campaigns/:campaign-id"
              ],
              "variable": [
                {
                  "id": "campaign-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Campaign"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a396321f-5491-48be-89cb-ea7b29848ae6"
            }
          ]
        },
        {
          "id": "9e95a3f6-1508-4d21-bff6-630e54a1718d",
          "name": "update-campaign",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/campaigns/:campaign-id"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "campaign-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update Campaign"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f837b29f-4476-4cd5-8f54-eb3d6f675c95"
            }
          ]
        },
        {
          "id": "d72aa43b-3c88-4f0d-a339-cf184d9e3932",
          "name": "delete-campaign",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/campaigns/:campaign-id"
              ],
              "variable": [
                {
                  "id": "campaign-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Campaign"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "956e9b84-f3a3-4ca3-bcc9-25e799c41cb5"
            }
          ]
        },
        {
          "id": "2c2f6d80-6de4-43f3-8a13-28ae98059078",
          "name": "get-campaign-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/campaigns/:campaign-id/events/"
              ],
              "variable": [
                {
                  "id": "campaign-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Campaign Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d22f73c5-4c73-4a92-8c4b-985eb1dac063"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "030b878e-0912-4a06-985f-70ac0a6c57dd",
          "name": "add-contact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add Contact"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d39cd4c8-8c7a-4c25-9b54-718840fb9ed8"
            }
          ]
        },
        {
          "id": "584c6f8b-971e-4646-ac9f-f6b6a2829bb7",
          "name": "get-contact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts/:contact-id"
              ],
              "variable": [
                {
                  "id": "contact-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Contact"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8fd120de-3191-4252-b21a-001190d494ad"
            }
          ]
        },
        {
          "id": "9df88298-1bd8-469c-847d-1a25ee721e6e",
          "name": "update-contact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts/:contact-id"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contact-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update Contact"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8eaf2c5-451f-4a65-9c12-52e4034f876d"
            }
          ]
        }
      ]
    },
    {
      "name": "Opting-out",
      "item": [
        {
          "id": "9cd6dd7d-5fde-4eb4-9c26-1c2d8afec279",
          "name": "optingout-contact",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts/:contact-id"
              ],
              "variable": [
                {
                  "id": "contact-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Opting-out Contact"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81e3b85a-724c-4e99-a6ee-aa60f077915b"
            }
          ]
        }
      ]
    },
    {
      "name": "Per-Contact",
      "item": [
        {
          "id": "4975e00d-3414-4d85-b0fd-66a5346d782b",
          "name": "get-percontact-campaign-events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/contacts/:contact-id/events/"
              ],
              "variable": [
                {
                  "id": "contact-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Per-Contact Campaign Events"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bcfbd6d-ec62-4a0d-8bd1-08325aa3c061"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "7463bc65-0d35-4ad4-b972-2e653fe49788",
          "name": "add-event",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/events"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Add Event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c8c7e67-1eeb-4190-9894-970a931dba3b"
            }
          ]
        },
        {
          "id": "1883101f-5934-440d-a878-dd6be4549b65",
          "name": "get-event",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/events/:event-id"
              ],
              "variable": [
                {
                  "id": "event-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd6889b5-26ab-4a7b-892b-e1409a298829"
            }
          ]
        }
      ]
    }
  ]
}