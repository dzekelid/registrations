{
  "info": {
    "name": "Microsoft Graph API List Registered Devices",
    "_postman_id": "58808b5f-a79d-4526-891d-bfb3835635ad",
    "description": "List registeredDevices Get the list of user's registered devices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "8c51071b-529d-498d-b9e4-78f67c231c80",
          "name": "ListRegisteredDevices",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/registeredDevices"
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List registeredDevices Get the list of user's registered devices"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "f2b290b1-4691-4e9b-96a9-36219f1b184a"
            }
          ]
        }
      ]
    }
  ]
}