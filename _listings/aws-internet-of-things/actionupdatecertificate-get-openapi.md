---
swagger: "2.0"
x-collection-name: AWS Internet of Things
x-complete: 0
info:
  title: AWS Internet of Things API Update Certificate
  version: 1.0.0
  description: Updates the status of the specified certificate.
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
  /?Action=CreateKeysAndCertificate:
    get:
      summary: Create Keys And Certificate
      description: Creates a 2048-bit RSA key pair and issues an X.
      operationId: createKeysAndCertificate
      x-api-path-slug: actioncreatekeysandcertificate-get
      parameters:
      - in: query
        name: setAsActive
        description: Specifies whether the certificate is active
        type: string
      responses:
        200:
          description: OK
      tags:
      - Keys And Certificates
  /?Action=DeleteCACertificate:
    get:
      summary: Delete C A Certificate
      description: Deletes a registered CA certificate.
      operationId: deleteCACertificate
      x-api-path-slug: actiondeletecacertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
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
  /?Action=DescribeCACertificate:
    get:
      summary: Describe C A Certificate
      description: Describes a registered CA certificate.
      operationId: describeCACertificate
      x-api-path-slug: actiondescribecacertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The CA certificate identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
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
  /?Action=ListCACertificates:
    get:
      summary: List C A Certificates
      description: Lists the CA certificates registered for your AWS account.
      operationId: listCACertificates
      x-api-path-slug: actionlistcacertificates-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Determines the order of the results
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
      - CA Certificates
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
  /?Action=ListCertificatesByCA:
    get:
      summary: List Certificates By C A
      description: List the device certificates signed by the specified CA certificate.
      operationId: listCertificatesByCA
      x-api-path-slug: actionlistcertificatesbyca-get
      parameters:
      - in: query
        name: ascendingOrder
        description: Specifies the order for results
        type: string
      - in: query
        name: caCertificateId
        description: The ID of the CA certificate
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
      - CA Certificates
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
  /?Action=RegisterCACertificate:
    get:
      summary: Register C A Certificate
      description: Registers a CA certificate with AWS IoT.
      operationId: registerCACertificate
      x-api-path-slug: actionregistercacertificate-get
      parameters:
      - in: query
        name: allowAutoRegistration
        description: Allows this CA certificate to be used for auto registration of
          device certificates
        type: string
      - in: query
        name: caCertificate
        description: The CA certificate
        type: string
      - in: query
        name: setAsActive
        description: A boolean value that specifies if the CA certificate is set to
          active
        type: string
      - in: query
        name: verificationCertificate
        description: The private key verification certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
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
  /?Action=UpdateCACertificate:
    get:
      summary: Update C A Certificate
      description: Updates a registered CA certificate.
      operationId: updateCACertificate
      x-api-path-slug: actionupdatecacertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The CA certificate identifier
        type: string
      - in: query
        name: newAutoRegistrationStatus
        description: The new value for the auto registration status
        type: string
      - in: query
        name: newStatus
        description: The updated status of the CA certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - CA Certificates
  /?Action=UpdateCertificate:
    get:
      summary: Update Certificate
      description: Updates the status of the specified certificate.
      operationId: updateCertificate
      x-api-path-slug: actionupdatecertificate-get
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      - in: query
        name: newStatus
        description: The new status
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