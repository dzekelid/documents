---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Starts download of contract document
  description: Starts download of contract document.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/accounts/contacts/{contactId}/document:
    get:
      summary: Get a single storage object from contact documents
      description: Get a single storage object from contact documents.
      operationId: getRestAccountsContactsContactDocument
      x-api-path-slug: restaccountscontactscontactiddocument-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key of the object to get from contact documents
      responses:
        200:
          description: OK
      tags:
      - Single
      - Storage
      - Object
      - From
      - Contact
      - Documents
    post:
      summary: Upload a document to contact directory
      description: Upload a document to contact directory.
      operationId: postRestAccountsContactsContactDocument
      x-api-path-slug: restaccountscontactscontactiddocument-post
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key for the file to upload
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Document
      - To
      - Contact
      - Directory
  /rest/accounts/contacts/{contactId}/documents:
    delete:
      summary: Delete files from contact documents
      description: Delete files from contact documents.
      operationId: deleteRestAccountsContactsContactDocuments
      x-api-path-slug: restaccountscontactscontactiddocuments-delete
      parameters:
      - in: path
        name: contactId
      - in: query
        name: keyList
        description: List of storage keys to delete
      responses:
        200:
          description: OK
      tags:
      - Files
      - From
      - Contact
      - Documents
  /rest/categories/{categoryId}/documents:
    get:
      summary: List documents of a category
      description: Lists the documents of a category. The ID of the category must
        be specified.
      operationId: getRestCategoriesCategoryDocuments
      x-api-path-slug: restcategoriescategoryiddocuments-get
      parameters:
      - in: path
        name: categoryId
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Category
    post:
      summary: Upload category documents
      description: Uploads documents to a category. The ID of the category must be
        specified.
      operationId: postRestCategoriesCategoryDocuments
      x-api-path-slug: restcategoriescategoryiddocuments-post
      parameters:
      - in: body
        name: /rest/categories/{categoryId}/documents
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryId
      - in: query
        name: directoryId
        description: The directory ID
      - in: query
        name: displayDate
        description: The date displayed on the document
      - in: query
        name: documents
        description: The array with the category documents
      - in: query
        name: number
        description: The document number
      - in: query
        name: numberWithPrefix
        description: Number with prefix
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Category
      - Documents
  /rest/categories/{categoryId}/documents/downloads:
    get:
      summary: Download category documents
      description: Downloads the documents of a category as a zip file. The ID of
        the category must be specified.
      operationId: getRestCategoriesCategoryDocumentsDownloads
      x-api-path-slug: restcategoriescategoryiddocumentsdownloads-get
      parameters:
      - in: path
        name: categoryId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Category
      - Documents
  /rest/orders/documents/downloads/{type}:
    get:
      summary: Download documents of a document type
      description: Downloads documents of the same document type as a zip file. The
        type of the documents must be specified.
      operationId: getRestOrdersDocumentsDownloadsType
      x-api-path-slug: restordersdocumentsdownloadstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: query
        name: itemsPerPage
        description: The number of documents to display per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: plentyId
        description: The plenty ID of the order documents
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Download
      - Documents
      - Of
      - Document
      - Type
  /rest/orders/documents/{type}:
    get:
      summary: List documents of a type
      description: Lists documents of a type. The type must be specified.
      operationId: getRestOrdersDocumentsType
      x-api-path-slug: restordersdocumentstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: query
        name: itemsPerPage
        description: The items per page to search for
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: type
      - in: query
        name: with
        description: Load additional relations for a document
      - in: query
        name: withContent
        description: Load also the document content as base64 encoded string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Type
  /rest/orders/shipping/export_documents/{orderId}:
    get:
      summary: List export documents by order ID
      description: List export documents by order id.
      operationId: getRestOrdersShippingExportDocumentsOrder
      x-api-path-slug: restordersshippingexport-documentsorderid-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Export
      - Documents
      - By
      - Order
      - ID
  /rest/orders/{orderId}/documents/downloads/{type?}:
    get:
      summary: Download documents of an order
      description: Downloads documents of an order as a zip file. The ID of the order
        must be specified. In addition a type can be specified.
      operationId: getRestOrdersOrderDocumentsDownloadsType
      x-api-path-slug: restordersorderiddocumentsdownloadstype-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: type
        description: The type of the document
      - in: path
        name: type?
      responses:
        200:
          description: OK
      tags:
      - Download
      - Documents
      - Of
      - Order
  /rest/orders/{orderId}/documents/{type?}:
    get:
      summary: List documents of an order
      description: Lists documents of an order. The ID of the order must be specified.
        In addition a type can be specified.
      operationId: getRestOrdersOrderDocumentsType
      x-api-path-slug: restordersorderiddocumentstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: path
        name: orderId
      - in: query
        name: type
        description: The type of the order documents
      - in: path
        name: type?
      - in: query
        name: with
        description: Load additional relations for a document
      - in: query
        name: withContent
        description: Load also the document content as base64 encoded string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Order
  /rest/orders/{orderId}/documents/{type}:
    post:
      summary: Upload order documents
      description: Uploads order documents. The ID of the order and the document type
        must be specified.
      operationId: postRestOrdersOrderDocumentsType
      x-api-path-slug: restordersorderiddocumentstype-post
      parameters:
      - in: body
        name: /rest/orders/{orderId}/documents/{type}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: orderId
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Order
      - Documents
  /rest/storage/layout:
    delete:
      summary: Delete layout documents
      description: Deletes a list of layout documents from storage. A list of storage
        keys must be specified.
      operationId: deleteRestStorageLayout
      x-api-path-slug: reststoragelayout-delete
      parameters:
      - in: query
        name: keyList
        description: List of storage keys for the files to be deleted
      responses:
        200:
          description: OK
      tags:
      - Layout
      - Documents
    post:
      summary: Upload a layout document
      description: Uploads a layout document to storage. The storage key (i.e. file
        path) must be specified.
      operationId: postRestStorageLayout
      x-api-path-slug: reststoragelayout-post
      parameters:
      - in: query
        name: key
        description: The storage key for the layout document to upload
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Layout
      - Document
  /rest/storage/layout/list:
    get:
      summary: List layout documents
      description: |-
        Lists up to 1000 layout documents per request. If more than 1000 layout documents are available,
        a <code>nextContinuationToken</code> is returned. Use this token to get the next (up to) 1000 layout documents.
        Use the same request and include a field with the key <code>continuationToken</code> as well as the returned
        token from the previous call as the value.

        Check the <code>isTruncated</code> field in the response to see if more results are available. If <code>isTruncated</code> is true,
        repeat the request using the token from the <code>nextContinuationToken</code> field of the previous response to get all
        results.
      operationId: getRestStorageLayoutList
      x-api-path-slug: reststoragelayoutlist-get
      parameters:
      - in: query
        name: continuationToken
        description: Token for listing the next (up to) 1000 layout documents
      responses:
        200:
          description: OK
      tags:
      - List
      - Layout
      - Documents
  /rest/accounts/contacts/{contactId}/document/url:
    get:
      summary: Get a temporary url for a single document
      description: Get a temporary url for a single document.
      operationId: getRestAccountsContactsContactDocumentUrl
      x-api-path-slug: restaccountscontactscontactiddocumenturl-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: key
        description: The storage key to get temporary url for
      responses:
        200:
          description: OK
      tags:
      - Temporary
      - Urla
      - Single
      - Document
  /rest/categories/{categoryId}/documents/{documentId}:
    delete:
      summary: Deletes a category document. The ID of the document must be specified.
      description: Deletes a category document. the id of the document must be specified..
      operationId: deleteRestCategoriesCategoryDocumentsDocument
      x-api-path-slug: restcategoriescategoryiddocumentsdocumentid-delete
      parameters:
      - in: path
        name: categoryId
      - in: path
        name: documentId
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
      - Document
      - ""
      - ID
      - Of
      - Document
      - Must
      - Be
      - Specified
  /rest/customer_contracts/{contractId}/document:
    get:
      summary: Starts download of contract document
      description: Starts download of contract document.
      operationId: getRestCustomerContractsContractDocument
      x-api-path-slug: restcustomer-contractscontractiddocument-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Download
      - Of
      - Contract
      - Document
  /rest/customer_contracts/{contractId}/sign/document:
    get:
      summary: Starts download of signed contract document
      description: Starts download of signed contract document.
      operationId: getRestCustomerContractsContractSignDocument
      x-api-path-slug: restcustomer-contractscontractidsigndocument-get
      parameters:
      - in: path
        name: contractId
      responses:
        200:
          description: OK
      tags:
      - Starts
      - Download
      - Of
      - Signed
      - Contract
      - Document
  /rest/documents/{documentId}:
    get:
      summary: Download the content of a document
      description: Downloads the content of a document. The ID of the document must
        be specified.
      operationId: getRestDocumentsDocument
      x-api-path-slug: restdocumentsdocumentid-get
      parameters:
      - in: path
        name: documentId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Content
      - Of
      - Document
  /rest/orders/documents/accounting_summary:
    get:
      summary: List document accounting summaries
      description: Lists document accounting summaries. A document accounting summary
        is saved along with each reversal document (for invoice and credit note).
        It contains accounting information about the order for this point in time.
        The summary is saved because an order can be updated after a reversal_document
        is generated. The information about the order before the update is needed
        for accounting.
      operationId: getRestOrdersDocumentsAccountingSummary
      x-api-path-slug: restordersdocumentsaccounting-summary-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: documentType
        description: The document type
      - in: query
        name: itemsPerPage
        description: The number of summaries to be displayed per page
      - in: query
        name: orderId
        description: The ID of the order
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Document
      - Accounting
      - Summaries
  /rest/storage/frontend/object-url:
    get:
      summary: Get the URL for a layout document
      description: Gets the URL of a layout document. The storage key must be specified.
        The returned URL expires after 10 minutes.
      operationId: getRestStorageFrontendObjectUrl
      x-api-path-slug: reststoragefrontendobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the frontend document to retrieve the URL
          for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Layout
      - Document
  /rest/storage/layout/object-url:
    get:
      summary: Get the URL for a layout document
      description: Gets the URL of a layout document. The storage key must be specified.
        The returned URL expires after 10 minutes.
      operationId: getRestStorageLayoutObjectUrl
      x-api-path-slug: reststoragelayoutobjecturl-get
      parameters:
      - in: query
        name: key
        description: The storage key for the layout document to retrieve the URL for
      responses:
        200:
          description: OK
      tags:
      - URLa
      - Layout
      - Document
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