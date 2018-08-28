swagger: "2.0"
x-collection-name: Azure Recovery Services
x-complete: 1
info:
  title: RecoveryServicesClient
  version: 1.0.0
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