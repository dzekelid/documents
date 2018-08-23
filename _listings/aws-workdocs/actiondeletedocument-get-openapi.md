---
swagger: "2.0"
x-collection-name: AWS WorkDocs
x-complete: 0
info:
  title: AWS WorkDocs API Delete Document
  version: 1.0.0
  description: Permanently deletes the specified document and its associated metadata.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AbortDocumentVersionUpload:
    get:
      summary: Abort Document Version Upload
      description: Aborts the upload of the specified document version that was previously
        initiated by.
      operationId: abortDocumentVersionUpload
      x-api-path-slug: actionabortdocumentversionupload-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      - in: query
        name: VersionId
        description: The ID of the version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
  /?Action=DeleteDocument:
    get:
      summary: Delete Document
      description: Permanently deletes the specified document and its associated metadata.
      operationId: deleteDocument
      x-api-path-slug: actiondeletedocument-get
      parameters:
      - in: query
        name: DocumentId
        description: The ID of the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Documents
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