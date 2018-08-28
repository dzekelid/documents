---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Create Document
  version: 1.0.0
  description: Creates an SSM document.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListDocuments:
    get:
      summary: List Documents
      description: Describes one or more of your SSM documents.
      operationId: listDocuments
      x-api-path-slug: actionlistdocuments-get
      parameters:
      - in: query
        name: DocumentFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
  /?Action=CreateDocument:
    get:
      summary: Create Document
      description: Creates an SSM document.
      operationId: createDocument
      x-api-path-slug: actioncreatedocument-get
      parameters:
      - in: query
        name: Content
        description: A valid JSON string
        type: string
      - in: query
        name: DocumentType
        description: The type of document to create
        type: string
      - in: query
        name: Name
        description: A name for the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=DeleteDocument:
    get:
      summary: Delete Document
      description: Deletes the SSM document and all instance associations to the document.
      operationId: deleteDocument
      x-api-path-slug: actiondeletedocument-get
      parameters:
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=DescribeDocument:
    get:
      summary: Describe Document
      description: Describes the specified SSM document.
      operationId: describeDocument
      x-api-path-slug: actiondescribedocument-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The document version for which you want information
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=DescribeDocumentPermission:
    get:
      summary: Describe Document Permission
      description: Describes the permissions for an SSM document.
      operationId: describeDocumentPermission
      x-api-path-slug: actiondescribedocumentpermission-get
      parameters:
      - in: query
        name: Name
        description: The name of the document for which you are the owner
        type: string
      - in: query
        name: PermissionType
        description: The permission type for the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
      - Permission
  /?Action=GetDocument:
    get:
      summary: Get Document
      description: Gets the contents of the specified SSM document.
      operationId: getDocument
      x-api-path-slug: actiongetdocument-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The document version for which you want information
        type: string
      - in: query
        name: Name
        description: The name of the SSM document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=ListDocumentVersions:
    get:
      summary: List Document Versions
      description: List all versions for a document.
      operationId: listDocumentVersions
      x-api-path-slug: actionlistdocumentversions-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: Name
        description: The name of the document about which you want version information
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Document
      - Versions
  /?Action=ModifyDocumentPermission:
    get:
      summary: Modify Document Permission
      description: Share a document publicly or privately.
      operationId: modifyDocumentPermission
      x-api-path-slug: actionmodifydocumentpermission-get
      parameters:
      - in: query
        name: AccountIdsToAdd
        description: The AWS user accounts that should have access to the document
        type: string
      - in: query
        name: AccountIdsToRemove
        description: The AWS user accounts that should no longer have access to the
          document
        type: string
      - in: query
        name: Name
        description: The name of the document that you want to share
        type: string
      - in: query
        name: PermissionType
        description: The permission type for the document
        type: string
      responses:
        200:
          description: OK
      tags:
      - Modify
      - Document
      - Permission
  /?Action=UpdateDocument:
    get:
      summary: Update Document
      description: The document you want to update.
      operationId: updateDocument
      x-api-path-slug: actionupdatedocument-get
      parameters:
      - in: query
        name: Content
        description: The content in a document that you want to update
        type: string
      - in: query
        name: DocumentVersion
        description: The version of the document that you want to update
        type: string
      - in: query
        name: Name
        description: The name of the document that you want to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
  /?Action=UpdateDocumentDefaultVersion:
    get:
      summary: Update Document Default Version
      description: Set the default version of a document.
      operationId: updateDocumentDefaultVersion
      x-api-path-slug: actionupdatedocumentdefaultversion-get
      parameters:
      - in: query
        name: DocumentVersion
        description: The version of a custom document that you want to set as the
          default version
        type: string
      - in: query
        name: Name
        description: The name of a custom document that you want to set as the default
          version
        type: string
      responses:
        200:
          description: OK
      tags:
      - Document
      - Default
      - Version
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