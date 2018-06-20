{
  "info": {
    "name": "reverb Get Webhooks Registrations",
    "_postman_id": "c3c551d0-5621-42b9-8b56-2cf143529482",
    "description": "Get webhooks registrations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhooks",
      "item": [
        {
          "id": "78d5fdb9-c63f-4a62-971a-131cfcceaf0e",
          "name": "getWebhooksRegistrations",
          "request": {
            "url": "http://api.reverb.com/api/webhooks/registrations",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get webhooks registrations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd742d59-1ffc-477f-b53d-e184f72f7033"
            }
          ]
        }
      ]
    }
  ]
}