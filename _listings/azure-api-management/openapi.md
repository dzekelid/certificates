---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 1
info:
  title: ApiManagementClient
  description: use-these-rest-apis-for-performing-operations-on-user-entity-in-azure-api-management-deployment--the-user-entity-in-api-management-represents-the-developers-that-call-the-apis-of-the-products-to-which-they-are-subscribed-
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/certificates
  : get:
      summary: Certificates ListByService
      description: Lists a collection of all certificates in the specified service
        instance.
      operationId: Certificates_ListByService
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamecertificates-get
      parameters:
      - in: query
        name: $filter
        description: '| Field          | Supported operators    | Supported functions                         ||----------------|------------------------|---------------------------------------------||
          id             | ge, le, eq, ne, gt, lt | substringof, contains, startswith,
          endswith || subject        | ge, le, eq, ne, gt, lt | substringof, contains,
          startswith, endswith || thumbprint     | ge, le, eq, ne, gt, lt | substringof,
          contains, startswith, endswith || expirationDate | ge, le, eq, ne, gt, lt
          | N/A                                         |'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Certificates
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ApiManagement/service/{serviceName}/certificates/{certificateId}
  : get:
      summary: Certificates Get
      description: Gets the details of the certificate specified by its identifier.
      operationId: Certificates_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamecertificatescertificateid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Certificates
    put:
      summary: Certificates CreateOrUpdate
      description: Creates or updates the certificate being used for authentication
        with the backend.
      operationId: Certificates_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamecertificatescertificateid-put
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the certificate to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Create parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Certificates
    delete:
      summary: Certificates Delete
      description: Deletes specific certificate.
      operationId: Certificates_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-apimanagementserviceservicenamecertificatescertificateid-delete
      parameters:
      - in: header
        name: If-Match
        description: The entity state (Etag) version of the certificate to delete
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Certificates
---