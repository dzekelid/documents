---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Documents
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - Get a single storage object from contact documents
  x-api-slug: restaccountscontactscontactiddocument-get
  description: Get a single storage object from contact documents.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocument-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocument-get-openapi.md
- name: plentymarkets REST-API - Delete files from contact documents
  x-api-slug: restaccountscontactscontactiddocuments-delete
  description: Delete files from contact documents.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocuments-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocuments-delete-openapi.md
- name: plentymarkets REST-API - List documents of a category
  x-api-slug: restcategoriescategoryiddocuments-get
  description: Lists the documents of a category. The ID of the category must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcategoriescategoryiddocuments-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcategoriescategoryiddocuments-get-openapi.md
- name: plentymarkets REST-API - Upload category documents
  x-api-slug: restcategoriescategoryiddocuments-post
  description: Uploads documents to a category. The ID of the category must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcategoriescategoryiddocuments-post-openapi.md
- name: plentymarkets REST-API - Download category documents
  x-api-slug: restcategoriescategoryiddocumentsdownloads-get
  description: Downloads the documents of a category as a zip file. The ID of the
    category must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcategoriescategoryiddocumentsdownloads-get-openapi.md
- name: plentymarkets REST-API - Download documents of a document type
  x-api-slug: restordersdocumentsdownloadstype-get
  description: Downloads documents of the same document type as a zip file. The type
    of the documents must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersdocumentsdownloadstype-get-openapi.md
- name: plentymarkets REST-API - List documents of a type
  x-api-slug: restordersdocumentstype-get
  description: Lists documents of a type. The type must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersdocumentstype-get-openapi.md
- name: plentymarkets REST-API - List export documents by order ID
  x-api-slug: restordersshippingexport-documentsorderid-get
  description: List export documents by order id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersshippingexport-documentsorderid-get-openapi.md
- name: plentymarkets REST-API - Download documents of an order
  x-api-slug: restordersorderiddocumentsdownloadstype-get
  description: Downloads documents of an order as a zip file. The ID of the order
    must be specified. In addition a type can be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersorderiddocumentsdownloadstype-get-openapi.md
- name: plentymarkets REST-API - List documents of an order
  x-api-slug: restordersorderiddocumentstype-get
  description: Lists documents of an order. The ID of the order must be specified.
    In addition a type can be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersorderiddocumentstype-get-openapi.md
- name: plentymarkets REST-API - Upload order documents
  x-api-slug: restordersorderiddocumentstype-post
  description: Uploads order documents. The ID of the order and the document type
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersorderiddocumentstype-post-openapi.md
- name: plentymarkets REST-API - Delete layout documents
  x-api-slug: reststoragelayout-delete
  description: Deletes a list of layout documents from storage. A list of storage
    keys must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/reststoragelayout-delete-openapi.md
- name: plentymarkets REST-API - List layout documents
  x-api-slug: reststoragelayoutlist-get
  description: |-
    Lists up to 1000 layout documents per request. If more than 1000 layout documents are available,
    a <code>nextContinuationToken</code> is returned. Use this token to get the next (up to) 1000 layout documents.
    Use the same request and include a field with the key <code>continuationToken</code> as well as the returned
    token from the previous call as the value.

    Check the <code>isTruncated</code> field in the response to see if more results are available. If <code>isTruncated</code> is true,
    repeat the request using the token from the <code>nextContinuationToken</code> field of the previous response to get all
    results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/reststoragelayoutlist-get-openapi.md
- name: plentymarkets REST-API - Upload a document to contact directory
  x-api-slug: restaccountscontactscontactiddocument-post
  description: Upload a document to contact directory.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocument-post-openapi.md
- name: plentymarkets REST-API - Get a temporary url for a single document
  x-api-slug: restaccountscontactscontactiddocumenturl-get
  description: Get a temporary url for a single document.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocumenturl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocumenturl-get-openapi.md
- name: plentymarkets REST-API - Deletes a category document. The ID of the document
    must be specified.
  x-api-slug: restcategoriescategoryiddocumentsdocumentid-delete
  description: Deletes a category document. the id of the document must be specified..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcategoriescategoryiddocumentsdocumentid-delete-openapi.md
- name: plentymarkets REST-API - Starts download of contract document
  x-api-slug: restcustomer-contractscontractiddocument-get
  description: Starts download of contract document.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcustomer-contractscontractiddocument-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcustomer-contractscontractiddocument-get-openapi.md
- name: plentymarkets REST-API - Starts download of signed contract document
  x-api-slug: restcustomer-contractscontractidsigndocument-get
  description: Starts download of signed contract document.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcustomer-contractscontractidsigndocument-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcustomer-contractscontractidsigndocument-get-openapi.md
- name: plentymarkets REST-API - Download the content of a document
  x-api-slug: restdocumentsdocumentid-get
  description: Downloads the content of a document. The ID of the document must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restdocumentsdocumentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restdocumentsdocumentid-get-openapi.md
- name: plentymarkets REST-API - List document accounting summaries
  x-api-slug: restordersdocumentsaccounting-summary-get
  description: Lists document accounting summaries. A document accounting summary
    is saved along with each reversal document (for invoice and credit note). It contains
    accounting information about the order for this point in time. The summary is
    saved because an order can be updated after a reversal_document is generated.
    The information about the order before the update is needed for accounting.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersdocumentsaccounting-summary-get-openapi.md
- name: plentymarkets REST-API - Download documents of a document type
  x-api-slug: restordersdocumentsdownloadstype-get
  description: Downloads documents of the same document type as a zip file. The type
    of the documents must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersdocumentsdownloadstype-get-openapi.md
- name: plentymarkets REST-API - Get the URL for a layout document
  x-api-slug: reststoragefrontendobjecturl-get
  description: Gets the URL of a layout document. The storage key must be specified.
    The returned URL expires after 10 minutes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/reststoragefrontendobjecturl-get-openapi.md
- name: plentymarkets REST-API - Upload a layout document
  x-api-slug: reststoragelayout-post
  description: Uploads a layout document to storage. The storage key (i.e. file path)
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/reststoragelayout-post-openapi.md
- name: plentymarkets REST-API - Get the URL for a layout document
  x-api-slug: reststoragelayoutobjecturl-get
  description: Gets the URL of a layout document. The storage key must be specified.
    The returned URL expires after 10 minutes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/reststoragelayoutobjecturl-get-openapi.md
- name: plentymarkets REST-API - Get the URL for a layout document
  x-api-slug: reststoragelayoutobjecturl-get
  description: Gets the URL of a layout document. The storage key must be specified.
    The returned URL expires after 10 minutes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/reststoragelayoutobjecturl-get-openapi.md
- name: plentymarkets REST-API - Upload a layout document
  x-api-slug: reststoragelayout-post
  description: Uploads a layout document to storage. The storage key (i.e. file path)
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/reststoragelayout-post-openapi.md
- name: plentymarkets REST-API - Get the URL for a layout document
  x-api-slug: reststoragefrontendobjecturl-get
  description: Gets the URL of a layout document. The storage key must be specified.
    The returned URL expires after 10 minutes.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/reststoragefrontendobjecturl-get-openapi.md
- name: plentymarkets REST-API - Download documents of a document type
  x-api-slug: restordersdocumentsdownloadstype-get
  description: Downloads documents of the same document type as a zip file. The type
    of the documents must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersdocumentsdownloadstype-get-openapi.md
- name: plentymarkets REST-API - List document accounting summaries
  x-api-slug: restordersdocumentsaccounting-summary-get
  description: Lists document accounting summaries. A document accounting summary
    is saved along with each reversal document (for invoice and credit note). It contains
    accounting information about the order for this point in time. The summary is
    saved because an order can be updated after a reversal_document is generated.
    The information about the order before the update is needed for accounting.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restordersdocumentsaccounting-summary-get-openapi.md
- name: plentymarkets REST-API - Download the content of a document
  x-api-slug: restdocumentsdocumentid-get
  description: Downloads the content of a document. The ID of the document must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restdocumentsdocumentid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restdocumentsdocumentid-get-openapi.md
- name: plentymarkets REST-API - Starts download of signed contract document
  x-api-slug: restcustomer-contractscontractidsigndocument-get
  description: Starts download of signed contract document.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcustomer-contractscontractidsigndocument-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcustomer-contractscontractidsigndocument-get-openapi.md
- name: plentymarkets REST-API - Starts download of contract document
  x-api-slug: restcustomer-contractscontractiddocument-get
  description: Starts download of contract document.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcustomer-contractscontractiddocument-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcustomer-contractscontractiddocument-get-openapi.md
- name: plentymarkets REST-API - Deletes a category document. The ID of the document
    must be specified.
  x-api-slug: restcategoriescategoryiddocumentsdocumentid-delete
  description: Deletes a category document. the id of the document must be specified..
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restcategoriescategoryiddocumentsdocumentid-delete-openapi.md
- name: plentymarkets REST-API - Get a temporary url for a single document
  x-api-slug: restaccountscontactscontactiddocumenturl-get
  description: Get a temporary url for a single document.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocumenturl-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocumenturl-get-openapi.md
- name: plentymarkets REST-API - Upload a document to contact directory
  x-api-slug: restaccountscontactscontactiddocument-post
  description: Upload a document to contact directory.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/documents/master/_listings/plentymarkets/restaccountscontactscontactiddocument-post-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---