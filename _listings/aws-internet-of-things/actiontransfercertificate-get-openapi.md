---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Transfer Certificate
  version: 1.0.0
  description: Transfers the specified certificate to the specified AWS account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateCertificateFromCsr:
    get:
      summary: Create Certificate From Csr
      description: Creates an X.
      operationId: createCertificateFromCsr
      x-api-path-slug: actioncreatecertificatefromcsr-get
      parameters:
      - in: query
        name: certificateSigningRequest
        description: The certificate signing request (CSR)
        type: string
      - in: query
        name: setAsActive
        description: Specifies whether the certificate is active
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=DeleteCertificate:
    get:
      summary: Delete Certificate
      description: Deletes the specified certificate.
      operationId: deleteCertificate
      x-api-path-slug: actiondeletecertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=DescribeCertificate:
    get:
      summary: Describe Certificate
      description: Gets information about the specified certificate.
      operationId: describeCertificate
      x-api-path-slug: actiondescribecertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ListCertificates:
    get:
      summary: List Certificates
      description: Lists the certificates registered in your AWS account.
      operationId: listCertificates
      x-api-path-slug: actionlistcertificates-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=ListOutgoingCertificates:
    get:
      summary: List Outgoing Certificates
      description: Lists certificates that are being transfered but not yet accepted.
      operationId: listOutgoingCertificates
      x-api-path-slug: actionlistoutgoingcertificates-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: marker
        description: The marker for the next set of results
        type: string
      - in: query
        name: pageSize
        description: The result page size
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=RegisterCertificate:
    get:
      summary: Register Certificate
      description: Registers a device certificate with AWS IoT.
      operationId: registerCertificate
      x-api-path-slug: actionregistercertificate-get
      parameters:
      - in: query
        name: caCertificatePem
        description: The CA certificate used to sign the device certificate being
          registered
        type: string
      - in: query
        name: certificatePem
        description: The certificate data, in PEM format
        type: string
      - in: query
        name: setAsActive
        description: A boolean value that specifies if the CA certificate is set to
          active
        type: string
      - in: query
        name: status
        description: The status of the register certificate request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Certificates
  /?Action=TransferCertificate:
    get:
      summary: Transfer Certificate
      description: Transfers the specified certificate to the specified AWS account.
      operationId: transferCertificate
      x-api-path-slug: actiontransfercertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: targetAwsAccount
        description: The AWS account
        type: string
      - in: query
        name: transferMessage
        description: The transfer message
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