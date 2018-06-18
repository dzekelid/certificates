---
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
  ? /Subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.RecoveryServices/vaults/{vaultName}/certificates/{certificateName}
  : put:
      summary: Vault Certificates Create
      description: Upload a certificate for a resource.
      operationId: VaultCertificates_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-recoveryservicesvaultsvaultnamecertificatescertificatename-put
      parameters:
      - in: path
        name: certificateName
        description: Certificate friendly name
      - in: body
        name: certificateRequest
        description: Input parameters for uploading the vault certificate
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Vault Certificates
---