swagger: "2.0"
x-collection-name: AWS Redshift
x-complete: 1
info:
  title: AWS Redshift API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeHsmClientCertificates:
    get:
      summary: Describe Hsm Client Certificates
      description: Returns information about the specified HSM client certificate.
      operationId: describeHsmClientCertificates
      x-api-path-slug: actiondescribehsmclientcertificates-get
      parameters:
      - in: query
        name: HsmClientCertificateIdentifier
        description: The identifier of a specific HSM client certificate for which
          you want information
        type: string
      - in: query
        name: Marker
        description: An optional parameter that specifies the starting point to return
          a set of response            records
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of response records to return in each call
        type: string
      - in: query
        name: TagKeys.TagKey.N
        description: A tag key or keys for which you want to return all matching HSM
          client certificates            that are associated with the specified key
          or keys
        type: string
      - in: query
        name: TagValues.TagValue.N
        description: A tag value or values for which you want to return all matching
          HSM client            certificates that are associated with the specified
          tag value or values
        type: string
      responses:
        200:
          description: OK
      tags:
      - HSM Client Certificates