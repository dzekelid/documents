---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Download documents of a document type
  description: Downloads documents of the same document type as a zip file. The type
    of the documents must be specified.
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