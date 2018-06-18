---
name: AWS Identity and Access Management
x-slug: aws-identity-and-access-management
description: AWS Identity and Access Management (IAM) enables you to securely control
  access to AWS services and resources for your users. Using IAM, you can create and
  manage AWS users and groups, and use permissions to allow and deny their access
  to AWS resources.IAM is a feature of your AWS account offered at no additional charge.
  You will be charged only for use of other AWS services by your users.To get started
  using IAM, orif you have already registered with AWS, go to theAWS Management Consoleand
  get started with theseIAM Best Practices.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Certificates
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/apis.md
specificationVersion: "0.14"
apis:
- name: AWS Identity and Access Management API Delete Server Certificate
  x-api-slug: aws-identity-and-access-management-api
  description: Deletes the specified server certificate.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=DeleteServerCertificate
  tags: Server Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actiondeleteservercertificate-get-openapi.md
- name: AWS Identity and Access Management API Delete Signing Certificate
  x-api-slug: aws-identity-and-access-management-api
  description: Deletes a signing certificate associated with the specified IAM user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=DeleteSigningCertificate
  tags: Signing Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actiondeletesigningcertificate-get-openapi.md
- name: AWS Identity and Access Management API Get Server Certificate
  x-api-slug: aws-identity-and-access-management-api
  description: Retrieves information about the specified server certificate stored
    in IAM.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=GetServerCertificate
  tags: Server Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actiongetservercertificate-get-openapi.md
- name: AWS Identity and Access Management API List Server Certificates
  x-api-slug: aws-identity-and-access-management-api
  description: Lists the server certificates stored in IAM that have the specified
    path prefix.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=ListServerCertificates
  tags: Serve rCertificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actionlistservercertificates-get-openapi.md
- name: AWS Identity and Access Management API List Signing Certificates
  x-api-slug: aws-identity-and-access-management-api
  description: |-
    Returns information about the signing certificates associated with the specified IAM
          user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=ListSigningCertificates
  tags: Signing Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actionlistsigningcertificates-get-openapi.md
- name: AWS Identity and Access Management API Update Server Certificate
  x-api-slug: aws-identity-and-access-management-api
  description: |-
    Updates the name and/or the path of the specified server certificate stored in
          IAM.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=UpdateServerCertificate
  tags: Server Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actionupdateservercertificate-get-openapi.md
- name: AWS Identity and Access Management API Update Signing Certificate
  x-api-slug: aws-identity-and-access-management-api
  description: |-
    Changes the status of the specified user signing certificate from active to disabled,
          or vice versa.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=UpdateSigningCertificate
  tags: Signing Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actionupdatesigningcertificate-get-openapi.md
- name: AWS Identity and Access Management API Upload Server Certificate
  x-api-slug: aws-identity-and-access-management-api
  description: Uploads a server certificate entity for the AWS account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=UploadServerCertificate
  tags: Server Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actionuploadservercertificate-get-openapi.md
- name: AWS Identity and Access Management API Upload Signing Certificate
  x-api-slug: aws-identity-and-access-management-api
  description: Uploads an X.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: ://///?Action=UploadSigningCertificate
  tags: Signing Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/actionuploadsigningcertificate-get-openapi.md
- name: AWS Identity and Access Management API
  x-api-slug: aws-identity-and-access-management-api
  description: AWS Identity and Access Management (IAM) enables you to securely control
    access to AWS services and resources for your users. Using IAM, you can create
    and manage AWS users and groups, and use permissions to allow and deny their access
    to AWS resources.IAM is a feature of your AWS account offered at no additional
    charge. You will be charged only for use of other AWS services by your users.To
    get started using IAM, orif you have already registered with AWS, go to theAWS
    Management Consoleand get started with theseIAM Best Practices.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Security-Identity_AWSIAM.png
  humanURL: https://aws.amazon.com/iam/
  baseURL: :///
  tags: Certificates
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/certificates/master/_listings/aws-identity-and-access-management/openapi.md
x-common:
- type: x-change-log
  url: http://developer.amazonwebservices.com/connect/kbcategory.jspa?categoryID=323
- type: x-command-line-interface
  url: http://docs.aws.amazon.com/cli/latest/reference/sts/index.html
- type: x-documentation
  url: http://docs.aws.amazon.com/IAM/latest/APIReference/
- type: x-faq
  url: https://aws.amazon.com/iam/faqs/
- type: x-forum
  url: https://forums.aws.amazon.com/forum.jspa?forumID=76
- type: x-getting-started
  url: https://aws.amazon.com/iam/getting-started/
- type: x-partners
  url: https://aws.amazon.com/iam/partners/
- type: x-tools
  url: http://aws.amazon.com/cli
- type: x-website
  url: https://aws.amazon.com/iam/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---