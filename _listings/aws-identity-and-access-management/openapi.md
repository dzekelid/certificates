---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 1
info:
  title: AWS Identity and Access Management API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListServerCertificates:
    get:
      summary: List Server Certificates
      description: Lists the server certificates stored in IAM that have the specified
        path prefix.
      operationId: listServerCertificates
      x-api-path-slug: actionlistservercertificates-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Serve rCertificates
  /?Action=ListSigningCertificates:
    get:
      summary: List Signing Certificates
      description: |-
        Returns information about the signing certificates associated with the specified IAM
              user.
      operationId: listSigningCertificates
      x-api-path-slug: actionlistsigningcertificates-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user whose signing certificates you want
          to examine
        type: string
      responses:
        200:
          description: OK
      tags:
      - Signing Certificates
---