{
  "info": {
    "name": "Azure Recovery Service API Registered Identities Delete",
    "_postman_id": "6f711052-871d-49bc-8086-66a57377e13a",
    "description": "Unregisters the given container from your Recovery Services vault.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "registered identities",
      "item": [
        {
          "id": "069dede5-4e32-49fa-84db-fb98e4d18559",
          "name": "RegisteredIdentities_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "Subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.RecoveryServices/vaults/:vaultName/registeredIdentities/:identityName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "identityName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "vaultName",
                  "value": "vaultName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Unregisters the given container from your Recovery Services vault"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "63ee0a7e-e2c0-462f-9dcf-fe50b50c3f4c"
            }
          ]
        }
      ]
    }
  ]
}