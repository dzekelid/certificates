---
swagger: "2.0"
x-collection-name: Azure API Management
x-complete: 0
info:
  title: Azure API Management API Certificates Get
  description: Gets the details of the certificate specified by its identifier.
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