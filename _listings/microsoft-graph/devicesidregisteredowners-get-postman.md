{
  "info": {
    "name": "Microsoft Graph API List Registered Owners",
    "_postman_id": "a2343cba-b764-4047-a33e-b49927e2a386",
    "description": "List registeredOwners Retrieve a list of users that are registered owners of the device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "1106fd7e-612a-426b-927e-ef5d6de9675d",
          "name": "ListRegisteredOwners",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "devices/:id/registeredOwners"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List registeredOwners Retrieve a list of users that are registered owners of the device"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "7725dd9b-43da-4a1d-b1dc-b33091f02848"
            }
          ]
        }
      ]
    }
  ]
}