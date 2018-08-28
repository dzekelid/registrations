---
swagger: "2.0"
x-collection-name: Azure Recovery Services
x-complete: 0
info:
  title: Azure Recovery Service API Registered Identities Delete
  version: 1.0.0
  description: Unregisters the given container from your Recovery Services vault.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/registeredIdentities/{identityName}
  : delete:
      summary: Registered Identities Delete
      description: Unregisters the given container from your Recovery Services vault.
      operationId: RegisteredIdentities_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnameregisteredidentitiesidentityname-delete
      parameters:
      - in: path
        name: identityName
        description: Name of the protection container to unregister
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Registered Identities
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---