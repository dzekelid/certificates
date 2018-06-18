---
name: AWS Certificate Manager
x-slug: aws-certificate-manager
description: AWS Certificate Manager is a service that lets you easily provision,
  manage, and deploy Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates
  for use with AWS services. SSL/TLS certificates are used to secure network communications
  and establish the identity of websites over the Internet. AWS Certificate Manager
  removes the time-consuming manual process of purchasing, uploading, and renewing
  SSL/TLS certificates. With AWS Certificate Manager, you can quickly request a certificate,
  deploy it on AWS resources such as Elastic Load Balancers or Amazon CloudFront distributions,
  and let AWS Certificate Manager handle certificate renewals. SSL/TLS certificates
  provisioned through AWS Certificate Manager are free. You pay only for the AWS resources
  you create to run your application.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Certificates
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-certificate-manager/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Certificate Manager API Delete Certificate
  x-api-slug: aws-certificate-manager-api
  description: Deletes an ACM Certificate and its associated private key.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=DeleteCertificate
  tags: Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-certificate-manager/actiondeletecertificate-get-openapi.md
- name: AWS Certificate Manager API Describe Certificate
  x-api-slug: aws-certificate-manager-api
  description: Returns a list of the fields contained in the specified ACM Certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=DescribeCertificate
  tags: Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-certificate-manager/actiondescribecertificate-get-openapi.md
- name: AWS Certificate Manager API Get Certificate
  x-api-slug: aws-certificate-manager-api
  description: |-
    Retrieves an ACM Certificate and certificate chain for the certificate specified by an
          ARN.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=GetCertificate
  tags: Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-certificate-manager/actiongetcertificate-get-openapi.md
- name: AWS Certificate Manager API Import Certificate
  x-api-slug: aws-certificate-manager-api
  description: Imports an SSL/TLS certificate into AWS Certificate Manager (ACM) to
    use with.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=ImportCertificate
  tags: Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-certificate-manager/actionimportcertificate-get-openapi.md
- name: AWS Certificate Manager API List Certificates
  x-api-slug: aws-certificate-manager-api
  description: Retrieves a list of ACM Certificates and the domain name for each.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=ListCertificates
  tags: Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-certificate-manager/actionlistcertificates-get-openapi.md
- name: AWS Certificate Manager API Request Certificate
  x-api-slug: aws-certificate-manager-api
  description: Requests an ACM Certificate for use with other AWS services.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: ://///?Action=RequestCertificate
  tags: Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-certificate-manager/actionrequestcertificate-get-openapi.md
- name: AWS Certificate Manager API
  x-api-slug: aws-certificate-manager-api
  description: AWS Certificate Manager is a service that lets you easily provision,
    manage, and deploy Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates
    for use with AWS services. SSL/TLS certificates are used to secure network communications
    and establish the identity of websites over the Internet. AWS Certificate Manager
    removes the time-consuming manual process of purchasing, uploading, and renewing
    SSL/TLS certificates. With AWS Certificate Manager, you can quickly request a
    certificate, deploy it on AWS resources such as Elastic Load Balancers or Amazon
    CloudFront distributions, and let AWS Certificate Manager handle certificate renewals.
    SSL/TLS certificates provisioned through AWS Certificate Manager are free. You
    pay only for the AWS resources you create to run your application.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_ACM_certificate-manager.png
  humanURL: https://aws.amazon.com/certificate-manager/
  baseURL: :///
  tags: Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-certificate-manager/openapi.md
x-common:
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/acm/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/acm/latest/APIReference/Welcome.html
- type: x-faq
  url: https://aws.amazon.com/certificate-manager/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=206
- type: x-getting-started
  url: https://aws.amazon.com/certificate-manager/getting-started/
- type: x-pricing
  url: https://aws.amazon.com/certificate-manager/pricing/
- type: x-website
  url: https://aws.amazon.com/certificate-manager/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---