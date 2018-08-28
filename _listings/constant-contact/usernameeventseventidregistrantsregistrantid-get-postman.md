{
  "info": {
    "name": "Constant Contact Get Registrant",
    "_postman_id": "c97e9bbd-6c7a-4f22-b6da-d47f3856be7d",
    "description": "Get Registrant",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "43496f84-c891-4e8e-b767-916f0f9c9ee4",
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
              "id": "33051db6-59d5-4462-ae01-72bb0666ba2f"
            }
          ]
        },
        {
          "id": "51532d95-6308-41e2-8873-ff51753ec299",
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
              "id": "5a1e1269-97ad-4103-9d5c-baeb4a27cdbf"
            }
          ]
        },
        {
          "id": "a427f186-c1a1-4acb-8336-ea7f42aab2c2",
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
              "id": "7e82dfe0-346a-492b-ac87-2e80ef68a24a"
            }
          ]
        },
        {
          "id": "a5ac107b-2975-453d-ad41-f253911952fb",
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
              "id": "606bda44-7faa-47ec-b169-29f19ee8f19d"
            }
          ]
        },
        {
          "id": "607288a3-ba36-4e46-b203-f91671dfa107",
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
              "id": "121021c3-e18a-4fe7-b370-d456756cdb45"
            }
          ]
        }
      ]
    },
    {
      "name": "Activity",
      "item": [
        {
          "id": "3901c3fe-e703-4c33-91b5-9bce3de0d7c7",
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
              "id": "8c612353-8e29-4477-b92e-f03da413b7e2"
            }
          ]
        },
        {
          "id": "ebdae02c-2e72-4f0a-be75-2ff089e589c7",
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
              "id": "a0bb0aa1-425d-4560-bc23-7f0448a190b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Campaign",
      "item": [
        {
          "id": "429129bd-d00b-4a25-b1b0-778bd9a4718c",
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
              "id": "6d74d4d6-d7e1-4168-9db7-c4ed786cae87"
            }
          ]
        },
        {
          "id": "49038d74-6566-4deb-a03a-e09dc394693f",
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
              "id": "5358ec78-fd2b-48ae-b358-3167a892f053"
            }
          ]
        },
        {
          "id": "08150459-e3eb-4c6a-be74-36319706cb57",
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
              "id": "ed743baf-ccb5-44c2-8384-15a7e9ba0677"
            }
          ]
        },
        {
          "id": "9e78703d-a376-4f76-ae19-5f9c070f9c96",
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
              "id": "c39e9ae9-4fa1-4388-9363-965f72530747"
            }
          ]
        },
        {
          "id": "83504122-bcfb-4708-aa78-39711e67eb31",
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
              "id": "f5563442-dc0f-4d42-874c-eee0664f1c80"
            }
          ]
        }
      ]
    },
    {
      "name": "Contact",
      "item": [
        {
          "id": "23eb509f-6a26-425a-b830-043299b386ee",
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
              "id": "6e2a5a98-9266-4761-90b8-b10eb60d3e38"
            }
          ]
        },
        {
          "id": "c57b591c-60fe-4d75-a075-bd5c355ce0b4",
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
              "id": "23d2b1be-0859-476f-b1a4-c27c5bb6fdb9"
            }
          ]
        },
        {
          "id": "2ac46a40-be19-4a57-bc11-c9a2dfa44325",
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
              "id": "5835f592-6293-4404-873e-e1d80970d670"
            }
          ]
        }
      ]
    },
    {
      "name": "Opting-out",
      "item": [
        {
          "id": "84d592a7-da49-4a59-b1e7-005d354936cc",
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
              "id": "24d61274-0127-466f-875f-53c0ea0a66b9"
            }
          ]
        }
      ]
    },
    {
      "name": "Per-Contact",
      "item": [
        {
          "id": "97425b7c-e697-402e-ae7c-87b9eefe306c",
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
              "id": "898256fe-76f0-4f22-aa84-75bf5922330e"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "2b7caed1-c573-4a90-9c6c-53e378ebab3e",
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
              "id": "14d120f4-22a3-4ea7-b422-b4fc0ab8a450"
            }
          ]
        },
        {
          "id": "7eba3f19-2775-4280-9995-9bfa9e99fbe6",
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
              "id": "5d7c81df-e330-424b-9817-dcf6106a40b6"
            }
          ]
        }
      ]
    },
    {
      "name": "Registrant",
      "item": [
        {
          "id": "57aff2b7-7783-4122-9f56-d864e2c832b7",
          "name": "get-registrant",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.constantcontact.com",
              "path": [
                "ws",
                "customers",
                ":username/events/:event-id/registrants/:registrant-id"
              ],
              "variable": [
                {
                  "id": "event-id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "registrant-id",
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
            "description": "Get Registrant"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb202731-8154-4cdb-9cc7-8b088665ce22"
            }
          ]
        }
      ]
    }
  ]
}