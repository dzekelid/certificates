---
swagger: "2.0"
x-collection-name: AWS API Gateway
x-complete: 0
info:
  title: AWS API Gateway API Clientcertificate Update
  version: 1.0.0
  description: Changes information about the ClientCertificate resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /clientcertificates/9ao60f:
    get:
      summary: Clientcertificate Byid
      description: Gets the ClientCertificate resource with the specified identifier.
      operationId: clientcertificateBy-id
      x-api-path-slug: clientcertificates9ao60f-get
      parameters:
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
      - Byid
  /clientcertificates:
    post:
      summary: Clientcertificate Generate
      description: Generates a new ClientCertificate resource.
      operationId: clientcertificateGenerate
      x-api-path-slug: clientcertificates-post
      parameters:
      - in: header
        name: '&quot;description&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: header
        name: Host
        type: string
      - in: header
        name: X-Amz-Date
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
      - Generate
  /clientcertificates/{clientcertificate_id}:
    patch:
      summary: Clientcertificate Update
      description: Changes information about the ClientCertificate resource.
      operationId: clientcertificateUpdate
      x-api-path-slug: clientcertificatesclientcertificate-id-patch
      parameters:
      - in: header
        name: '&quot;op&quot;'
        type: string
      - in: header
        name: '&quot;patchOperations&quot;'
        type: string
      - in: header
        name: '&quot;path&quot;'
        type: string
      - in: header
        name: '&quot;value&quot;'
        type: string
      - in: header
        name: Authorization
        type: string
      - in: header
        name: Content-Type
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: ExecutableBy.N
        description: Scopes the images by users with explicit launch permissions
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: body
        name: from
        description: Not supported
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Host
        type: string
      - in: query
        name: ImageId.N
        description: One or more image IDs
        type: string
      - in: body
        name: op
        description: An update operation to be performed with this PATCH request
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: Owner.N
        description: Filters the images by the owner
        type: string
      - in: body
        name: path
        description: The op operation&#39;s target, as identified by a JSON Pointer
          value that references a location within the targeted resource
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: value
        description: The new target value of the update operation
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: X-Amz-Date
        type: string
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