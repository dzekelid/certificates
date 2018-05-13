---
swagger: "2.0"
info:
  title: AWS Internet of Things API Describe Certificate
  version: 1.0.0
  description: Gets information about the specified certificate.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeCertificate:
    get:
      summary: ' Describe Certificate '
      description: Gets information about the specified certificate
      operationId: describeCertificate
      parameters:
      - in: query
        name: certificateId
        description: The ID of the certificate
        type: string
      responses:
        200:
          description: OK
      tags:
      - certificates
definitions: []
x-collection-name: AWS Internet of Things
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