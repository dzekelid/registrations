{
  "info": {
    "name": "Microsoft Graph API List Registered Users",
    "_postman_id": "6b23dcbd-ae75-4bd8-b8e4-0f39df3c80ed",
    "description": "List registeredUsers Retrieve a list of users that are registered users of the device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "list",
      "item": [
        {
          "id": "d5450ba3-cc40-407e-b31b-82e712e50fe0",
          "name": "ListRegisteredUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "devices/:id/registeredUsers"
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
            "description": "List registeredUsers Retrieve a list of users that are registered users of the device"
          },
          "response": [
            {
              "code": 200,
              "name": "Response_200",
              "id": "97a3420d-a6ff-4ab9-94ae-eb5a9f292a53"
            }
          ]
        }
      ]
    }
  ]
}