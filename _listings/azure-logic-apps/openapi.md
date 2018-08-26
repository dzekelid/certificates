---
swagger: "2.0"
x-collection-name: Azure Logic Apps
x-complete: 1
info:
  title: LogicManagementClient
  description: rest-api-for-azure-logic-apps-
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Logic/integrationAccounts/{integrationAccountName}/certificates/{certificateName}
  : get:
      summary: Certificates Get
      description: Gets an integration account certificate.
      operationId: Certificates_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamecertificatescertificatename-get
      parameters:
      - in: path
        name: certificateName
        description: The integration account certificate name
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Certificates
    put:
      summary: Certificates Create Or Update
      description: Creates or updates an integration account certificate.
      operationId: Certificates_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamecertificatescertificatename-put
      parameters:
      - in: body
        name: certificate
        description: The integration account certificate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: certificateName
        description: The integration account certificate name
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Certificates
    delete:
      summary: Certificates Delete
      description: Deletes an integration account certificate.
      operationId: Certificates_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-logicintegrationaccountsintegrationaccountnamecertificatescertificatename-delete
      parameters:
      - in: path
        name: certificateName
        description: The integration account certificate name
      - in: path
        name: integrationAccountName
        description: The integration account name
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The resource group name
      responses:
        200:
          description: OK
      tags:
      - Certificates
---