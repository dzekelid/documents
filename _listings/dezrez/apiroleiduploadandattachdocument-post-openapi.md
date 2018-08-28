---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Allows you to upload a document and attach it directly to a role.
  version: 1.0.0
  description: Allows you to upload a document and attach it directly to a role..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Document:
    get:
      summary: Get documents by their ids
      description: Get documents by their ids.
      operationId: Document_GetByids
      x-api-path-slug: apidocument-get
      parameters:
      - in: query
        name: ids
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Documents
      - By
      - Their
      - Ids
  /api/group/{id}/documents:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_DocumentsByidBysubTypesBypageSizeBypageNumberBytypeByorderDesc
      x-api-path-slug: apigroupiddocuments-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: orderDesc
        description: Order by created date descending (true by default)
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subTypes
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/group/{id}/offers/made:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_OffersMadeByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidoffersmade-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/group/{id}/offers/received:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_OffersReceivedByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidoffersreceived-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/property/{id}/documents:
    get:
      summary: Get the documents of a property by the property Id
      description: Get the documents of a property by the property id.
      operationId: Property_DocumentsByidBysubTypesBypageSizeBypageNumberBytype
      x-api-path-slug: apipropertyiddocuments-get
      parameters:
      - in: path
        name: id
        description: The id of the property to get the documents for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subTypes
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Of
      - Property
      - By
      - Property
      - Id
  /api/role/{id}/documents:
    get:
      summary: Get a list of documents belonging to a role
      description: Get a list of documents belonging to a role.
      operationId: Role_DocumentsByidBysubTypesBypageSizeBypageNumberBytypeByorderDesc
      x-api-path-slug: apiroleiddocuments-get
      parameters:
      - in: path
        name: id
        description: The id of the role to get the documents for
      - in: query
        name: orderDesc
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subTypes
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Role
  /api/roomdescription/setimages:
    post:
      summary: Allows you to specify a list of documentIds for a roomDescriptions
        room - this list will overwrite any existing list of documents on that room,
        and order will be honoured.
      description: Allows you to specify a list of documentids for a roomdescriptions
        room - this list will overwrite any existing list of documents on that room,
        and order will be honoured..
      operationId: RoomDescription_SetImagesByroomImageOrder
      x-api-path-slug: apiroomdescriptionsetimages-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: roomImageOrder
        description: The room image order
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Specify
      - List
      - Of
      - DocumentIdsa
      - RoomDescriptions
      - Room
      - '-'
      - This
      - List
      - Will
      - Overwrite
      - Any
      - Existing
      - List
      - Of
      - Documents
      - "On"
      - That
      - Room
      - ""
      - Order
      - Will
      - Be
      - Honoured
  /api/sync/mailsync:
    post:
      summary: Syncronise Email with Rezi Events, attach documents etc
      description: Syncronise email with rezi events, attach documents etc.
      operationId: Sync_EmailBymailSyncDataContract
      x-api-path-slug: apisyncmailsync-post
      parameters:
      - in: body
        name: mailSyncDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Syncronise
      - Email
      - Rezi
      - Events
      - ""
      - Attach
      - Documents
      - Etc
  /api/branding/{id}/attachexternaldocument:
    put:
      summary: Attaches an external document to brand.
      description: Attaches an external document to brand..
      operationId: Branding_AttachExternalDocumentByidByexternalDocument
      x-api-path-slug: apibrandingidattachexternaldocument-put
      parameters:
      - in: body
        name: externalDocument
        description: Details of the external document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - External
      - Document
      - To
      - Brand
  /api/branding/{id}/uploadandattachdocument:
    put:
      summary: Uploads and attaches a document to a brand.
      description: Uploads and attaches a document to a brand..
      operationId: Branding_UploadAndAttachDocumentByidBydocumentDetails
      x-api-path-slug: apibrandingiduploadandattachdocument-put
      parameters:
      - in: body
        name: documentDetails
        description: Details of the file
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/uploadandattachdocumenttodefault:
    put:
      summary: Uploads and attaches a document to a brand.
      description: Uploads and attaches a document to a brand..
      operationId: Branding_UploadAndAttachDocumentToDefaultBrandBydocumentDetailsByid
      x-api-path-slug: apibrandingiduploadandattachdocumenttodefault-put
      parameters:
      - in: body
        name: documentDetails
        description: Details of the file
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/attachdocument:
    put:
      summary: Attaches a document to a brand.
      description: Attaches a document to a brand..
      operationId: Branding_AttachDocumentByidBydocumentId
      x-api-path-slug: apibrandingidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The documentId
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Document
      - To
      - Brand
  /api/branding/{id}/detachdocument:
    put:
      summary: Detaches a document from a brand.
      description: Detaches a document from a brand..
      operationId: Branding_DetachDocumentByidBydocumentId
      x-api-path-slug: apibrandingiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The documentId
      - in: path
        name: id
        description: The BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Brand
  /api/branding/{id}/uploaddocumentcustomisation:
    put:
      summary: Upload the data to customise a Brand Document.
      description: Upload the data to customise a brand document..
      operationId: Branding_UploadDocumentCustomisationByidBycustomisationSaveData
      x-api-path-slug: apibrandingiduploaddocumentcustomisation-put
      parameters:
      - in: body
        name: customisationSaveData
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: BrandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Customise
      - Brand
      - Document
  /api/branding/uploadsmstemplate:
    post:
      summary: Upload the data to create a SMS Document Template for a Brand.
      description: Upload the data to create a sms document template for a brand..
      operationId: Branding_UploadSMSTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploadsmstemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - SMS
      - Document
      - Templatea
      - Brand
  /api/branding/uploademailtemplate:
    post:
      summary: Upload the data to create a Email Document Template for a Brand.
      description: Upload the data to create a email document template for a brand..
      operationId: Branding_UploadEmailTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploademailtemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - Email
      - Document
      - Templatea
      - Brand
  /api/digitalsignature/signable/opened/{fingerprint}:
    post:
      summary: creates an event when a document is opened
      description: Creates an event when a document is opened.
      operationId: DigitalSignature_OpenedByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignableopenedfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Opened
  /api/digitalsignature/signable/cancelled/{fingerprint}:
    post:
      summary: creates an event when a document is cancelled
      description: Creates an event when a document is cancelled.
      operationId: DigitalSignature_CancelledByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablecancelledfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Cancelled
  /api/digitalsignature/signable/sent/{fingerprint}:
    post:
      summary: creates an event when a document is sent out by signable
      description: Creates an event when a document is sent out by signable.
      operationId: DigitalSignature_SentByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablesentfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Sent
      - Out
      - By
      - Signable
  /api/digitalsignature/signable/signed/{fingerprint}:
    post:
      summary: creates an event when a document is signed
      description: Creates an event when a document is signed.
      operationId: DigitalSignature_SignedByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablesignedfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Signed
  /api/digitalsignature/signable/completed/{fingerprint}:
    post:
      summary: creates an event when a document is completed
      description: Creates an event when a document is completed.
      operationId: DigitalSignature_CompletedByfingerprintBymetaData
      x-api-path-slug: apidigitalsignaturesignablecompletedfingerprint-post
      parameters:
      - in: path
        name: fingerprint
      - in: body
        name: metaData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Event
      - When
      - Document
      - Is
      - Completed
  /api/document/{id}:
    get:
      summary: Gets a document by its id.
      description: Gets a document by its id..
      operationId: Document_GetByid
      x-api-path-slug: apidocumentid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Document
      - By
      - Its
      - Id
  /api/document/{id}/savedescription:
    put:
      summary: Save the document description. Used for the image caption for the portals.
      description: Save the document description. used for the image caption for the
        portals..
      operationId: Document_SaveDescriptionByidBydescription
      x-api-path-slug: apidocumentidsavedescription-put
      parameters:
      - in: query
        name: description
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Document
      - Description
      - ""
      - Usedthe
      - Image
      - Captionthe
      - Portals
  /api/document/setprivacy:
    put:
      summary: Sets the document privacy for an existing document.  This is used to
        change a document from being publicly accessible to being private, and vice
        versa.
      description: Sets the document privacy for an existing document.  this is used
        to change a document from being publicly accessible to being private, and
        vice versa..
      operationId: Document_SetDocumentPrivacyBysetDocumentPrivacyCommand
      x-api-path-slug: apidocumentsetprivacy-put
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setDocumentPrivacyCommand
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Document
      - Privacyan
      - Existing
      - Document
      - ""
      - ""
      - This
      - Is
      - Used
      - To
      - Change
      - Document
      - From
      - Being
      - Publicly
      - Accessible
      - To
      - Being
      - Private
      - ""
      - Vice
      - Versa
  /api/document/rename:
    put:
      summary: Updates the filename of an existing document.
      description: Updates the filename of an existing document..
      operationId: Document_RenameByrenameDocumentCommandDataContract
      x-api-path-slug: apidocumentrename-put
      parameters:
      - in: body
        name: renameDocumentCommandDataContract
        description: The new filename (excluding the extension)
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Filename
      - Of
      - Existing
      - Document
  /api/document/{id}/download:
    get:
      summary: Download a document by its id.
      description: Download a document by its id..
      operationId: Document_DownloadAsyncByid
      x-api-path-slug: apidocumentiddownload-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Download
      - Document
      - By
      - Its
      - Id
  /api/documentgeneration/bulkpropertyownercommunication:
    post:
      summary: "Generates a bulk communication pack out to multiple vendors of properties.\r\nThis
        will ignore the target type set, as the document could only ever find the
        vendor as the contact item, so it always defaults\r\nto a target type of vendor/owner"
      description: "Generates a bulk communication pack out to multiple vendors of
        properties.\r\nthis will ignore the target type set, as the document could
        only ever find the vendor as the contact item, so it always defaults\r\nto
        a target type of vendor/owner."
      operationId: DocumentGeneration_BulkPropertyVendorCommunicationBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationbulkpropertyownercommunication-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Bulk
      - Communication
      - Pack
      - Out
      - To
      - Multiple
      - Vendors
      - Of
      - Properties
      - This
      - Will
      - Ignore
      - Target
      - Type
      - Set
      - ""
      - As
      - Document
      - Could
      - Only
      - Ever
      - Find
      - Vendor
      - As
      - Contact
      - Item
      - ""
      - So
      - It
      - Always
      - "Defaults\r\nTo"
      - Target
      - Type
      - Of
      - Vendor
      - Owner
  /api/documentgeneration/envelopecontent/{sackReference}/{envelopereference}/{documentreference}:
    delete:
      summary: deletes an document from an envelope
      description: Deletes an document from an envelope.
      operationId: DocumentGeneration_DeleteEnvelopeContentBysackReferenceByenvelopereferenceBydocumentreference
      x-api-path-slug: apidocumentgenerationenvelopecontentsackreferenceenvelopereferencedocumentreference-delete
      parameters:
      - in: path
        name: documentreference
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Document
      - From
      - Envelope
  /api/documentgeneration/packrequiredtypes/{packid}:
    get:
      summary: Get a list of the packs required types (ie all of the types required
        by each document in each envelope)
      description: Get a list of the packs required types (ie all of the types required
        by each document in each envelope).
      operationId: DocumentGeneration_PackRequiredTypesBypackid
      x-api-path-slug: apidocumentgenerationpackrequiredtypespackid-get
      parameters:
      - in: path
        name: packid
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Packs
      - Required
      - Types
      - (ie
      - ""
      - Of
      - Types
      - Required
      - By
      - Each
      - Document
      - In
      - Each
      - Envelope)
  /api/documentgeneration/packsupportedsendmethods/{packid}:
    get:
      summary: Get a list of the supported sending methods for a correspondence (ie
        all of the types required by each document in each envelope)
      description: Get a list of the supported sending methods for a correspondence
        (ie all of the types required by each document in each envelope).
      operationId: DocumentGeneration_PackSupportedSendMethodsBypackid
      x-api-path-slug: apidocumentgenerationpacksupportedsendmethodspackid-get
      parameters:
      - in: path
        name: packid
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Supported
      - Sending
      - Methodsa
      - Correspondence
      - (ie
      - ""
      - Of
      - Types
      - Required
      - By
      - Each
      - Document
      - In
      - Each
      - Envelope)
  /api/documentgeneration/createpdf:
    post:
      summary: Creates a new pdf document.
      description: Creates a new pdf document..
      operationId: DocumentGeneration_CreatePdfBypdfData
      x-api-path-slug: apidocumentgenerationcreatepdf-post
      parameters:
      - in: body
        name: pdfData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Pdf
      - Document
  /api/documentgeneration/recreateepc:
    post:
      summary: Creates a new epc document.
      description: Creates a new epc document..
      operationId: DocumentGeneration_RecreateEpcByepcData
      x-api-path-slug: apidocumentgenerationrecreateepc-post
      parameters:
      - in: body
        name: epcData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Epc
      - Document
  /api/documentgeneration/recreatepropertymarketreport/{propertyId}:
    post:
      summary: Creates a new Property Market Report document.
      description: Creates a new property market report document..
      operationId: DocumentGeneration_RecreatePropertyMarketReportBypropertyId
      x-api-path-slug: apidocumentgenerationrecreatepropertymarketreportpropertyid-post
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Property
      - Market
      - Report
      - Document
  /api/documentgeneration/documentSubTypes:
    get:
      summary: Get the appropriate document sub types for a document type
      description: Get the appropriate document sub types for a document type.
      operationId: DocumentGeneration_getDocumentSubTypesByDocumentTypeSystemName
      x-api-path-slug: apidocumentgenerationdocumentsubtypes-get
      parameters:
      - in: query
        name: DocumentTypeSystemName
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Appropriate
      - Document
      - Sub
      - Typesa
      - Document
      - Type
  /api/group/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a group
      description: Attaches an existing document to a group.
      operationId: Group_AttachDocumentByidBydocumentId
      x-api-path-slug: apigroupidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the group to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Group
  /api/group/{id}/detachdocument:
    put:
      summary: Detaches a document from a group
      description: Detaches a document from a group.
      operationId: Group_DetachDocumentByidBydocumentId
      x-api-path-slug: apigroupiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the group to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Group
  /api/group/{id}/uploadandattachdocument:
    post:
      summary: Uploads a new document and attaches it to the specified group.
      description: Uploads a new document and attaches it to the specified group..
      operationId: Group_UploadAndAttachDocumentByidBydocumentDetails
      x-api-path-slug: apigroupiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetails
        description: The document details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - New
      - Document
      - Attaches
      - It
      - To
      - Specified
      - Group
  /api/group/{id}/attachexternaldocument:
    post:
      summary: Attaches the external document.
      description: Attaches the external document..
      operationId: Group_AttachExternalDocumentByidBydocumentDetails
      x-api-path-slug: apigroupidattachexternaldocument-post
      parameters:
      - in: body
        name: documentDetails
        description: The document details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - External
      - Document
  /api/progression/lettings/uploadandattachtenantdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a tenant.
      description: Allows you to upload a document and attach it directly to a tenant..
      operationId: LettingsProgression_UploadAndAttachTenantDocumentBytenantInfoIdBydocumentDetailsContract
      x-api-path-slug: apiprogressionlettingsuploadandattachtenantdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantInfoId
        description: The tenant Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Tenant
  /api/progression/lettings/uploadandattachlandlorddocument:
    post:
      summary: Allows you to upload a document and attach it directly to a tenant.
      description: Allows you to upload a document and attach it directly to a tenant..
      operationId: LettingsProgression_UploadAndAttachLandlordDocumentBylandlordInfoIdBydocumentDetailsContract
      x-api-path-slug: apiprogressionlettingsuploadandattachlandlorddocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: landlordInfoId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Tenant
  /api/progression/lettings/uploadandattachguarantorgroupdocument:
    post:
      summary: Allows you to upload a lettings document and attach it directly to
        a guarantor group.
      description: Allows you to upload a lettings document and attach it directly
        to a guarantor group..
      operationId: LettingsProgression_UploadAndAttachGurantorGroupDocumentByguarantorGroupIdBytenancyIdBydocumentDetai
      x-api-path-slug: apiprogressionlettingsuploadandattachguarantorgroupdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: guarantorGroupId
        description: The guarantor group Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenancyId
        description: The tenancy Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Lettings
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
      - Group
  /api/progression/lettings/detatchdocumentfromlandlord:
    post:
      summary: Detatch a document from a landlord.
      description: Detatch a document from a landlord..
      operationId: LettingsProgression_DetatchDocumentFromLandlordBylandlordInfoIdBydocumentId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromlandlord-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: query
        name: landlordInfoId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Landlord
  /api/progression/lettings/detatchdocumentfromtenant:
    post:
      summary: Detatch a document from a landlord.
      description: Detatch a document from a landlord..
      operationId: LettingsProgression_DetatchDocumentFromTenantBytenantInfoIdBydocumentId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromtenant-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantInfoId
        description: The tenant Id
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Landlord
  /api/progression/lettings/detatchdocumentfromguarantor:
    post:
      summary: Detatch a document from a landlord.
      description: Detatch a document from a landlord..
      operationId: LettingsProgression_DetatchDocumentFromGuarantorByguarantorIdBydocumentIdBypersonId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromguarantor-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: query
        name: guarantorId
        description: The tenant Id
      - in: query
        name: personId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Landlord
  /api/progression/lettings/detatchdocumentfromreference:
    post:
      summary: Detatch a document from a reference.
      description: Detatch a document from a reference..
      operationId: LettingsProgression_DetatchDocumentFromReferenceByreferenceIdBydocumentId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromreference-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: query
        name: referenceId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Reference
  /api/progression/lettings/uploadandattachguarantordocument:
    post:
      summary: Allows you to upload a document and attach it directly to a guarantor.
      description: Allows you to upload a document and attach it directly to a guarantor..
      operationId: LettingsProgression_UploadAndAttachGuarantorDocumentByguarantorIdBydocumentDetailsContract
      x-api-path-slug: apiprogressionlettingsuploadandattachguarantordocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: guarantorId
        description: The guarantor Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
  /api/progression/lettings/uploadandattachguarantorreferencedocument:
    post:
      summary: Allows you to upload a document and attach it directly to a guarantor.
      description: Allows you to upload a document and attach it directly to a guarantor..
      operationId: LettingsProgression_UploadAndAttachGuarantorReferenceDocumentByguarantorIdByreferenceIdBydocumentDet
      x-api-path-slug: apiprogressionlettingsuploadandattachguarantorreferencedocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: guarantorId
        description: The guarantor Id
      - in: query
        name: referenceId
        description: The reference Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
  /api/progression/lettings/uploadandattachrighttorentdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a r ight
        to rent.
      description: Allows you to upload a document and attach it directly to a r ight
        to rent..
      operationId: LettingsProgression_UploadAndAttachRightToRentDocumentBytenantInfoIdBydocumentDetailsContract
      x-api-path-slug: apiprogressionlettingsuploadandattachrighttorentdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantInfoId
        description: The tenant info Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - R
      - Ight
      - To
      - Rent
  /api/progression/lettings/uploadandattachtenantreferencedocument:
    post:
      summary: Allows you to upload a document and attach it directly to a guarantor.
      description: Allows you to upload a document and attach it directly to a guarantor..
      operationId: LettingsProgression_UploadAndAttachTenantReferenceDocumentBytenantInfoIdByreferenceIdBytenantRoleIdB
      x-api-path-slug: apiprogressionlettingsuploadandattachtenantreferencedocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: referenceId
        description: The reference Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantInfoId
        description: The tenantInfoId Id
      - in: query
        name: tenantRoleId
        description: The reference Id
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
  /api/milestone/{id}/uploadandattachdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a milestone.
      description: Allows you to upload a document and attach it directly to a milestone..
      operationId: Milestone_UploadAndAttachDocumentByidBydocumentDetailsContract
      x-api-path-slug: apimilestoneiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        description: Document save command
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The milestone Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Milestone
  /api/milestone/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a milestone
      description: Attaches an existing document to a milestone.
      operationId: Milestone_AttachDocumentByidBydocumentId
      x-api-path-slug: apimilestoneidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the milestone to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Milestone
  /api/milestone/{id}/detachdocument:
    put:
      summary: Detaches a document from a milestone
      description: Detaches a document from a milestone.
      operationId: Milestone_DetachDocumentByidBydocumentId
      x-api-path-slug: apimilestoneiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the milestone to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Milestone
  /api/property/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a property
      description: Attaches an existing document to a property.
      operationId: Property_AttachDocumentByidBydocumentId
      x-api-path-slug: apipropertyidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the property to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Property
  /api/property/{id}/detachdocument:
    put:
      summary: Detaches a document from a property
      description: Detaches a document from a property.
      operationId: Property_DetachDocumentByidBydocumentId
      x-api-path-slug: apipropertyiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the property description to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Property
  /api/property/{id}/uploadandattachdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a property.
      description: Allows you to upload a document and attach it directly to a property..
      operationId: Property_UploadAndAttachDocumentByidBydocumentDetailsContract
      x-api-path-slug: apipropertyiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        description: Details o
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Property
  /api/property/{id}/attachexternaldocument:
    post:
      summary: Attaches an externally hosted document to a property
      description: Attaches an externally hosted document to a property.
      operationId: Property_AttachExternalDocumentByidBydocumentDetails
      x-api-path-slug: apipropertyidattachexternaldocument-post
      parameters:
      - in: body
        name: documentDetails
        description: Details of the document to associate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The property Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Externally
      - Hosted
      - Document
      - To
      - Property
  /api/property/uploadandattachcertificatedocument:
    post:
      summary: Allows you to upload a document and attach it directly to a guarantor.
      description: Allows you to upload a document and attach it directly to a guarantor..
      operationId: Property_UploadAndAttachCertificateDocumentBycertificateIdBydocumentDetailsContract
      x-api-path-slug: apipropertyuploadandattachcertificatedocument-post
      parameters:
      - in: query
        name: certificateId
        description: The Certificate Id
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Guarantor
  /api/role/{id}/documentfromplaceholder:
    get:
      summary: Get a single DocumentPlaceholder which is the 'slot' the particular
        document of type+source exists within.
      description: Get a single documentplaceholder which is the 'slot' the particular
        document of type+source exists within..
      operationId: Role_DocumentFromPlaceholderByidByplaceholderTypeByplaceholderSourceTypeBygroupId
      x-api-path-slug: apiroleiddocumentfromplaceholder-get
      parameters:
      - in: query
        name: groupId
        description: Optional group id to filter placeholder for a specific group
          relating to this role
      - in: path
        name: id
        description: Role id
      - in: query
        name: placeholderSourceType
        description: Where did the document come from to fit into the placeholder
          slot
      - in: query
        name: placeholderType
        description: Which type of document placeholder slot is this
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Single
      - DocumentPlaceholder
      - Which
      - Is
      - Slot
      - Particular
      - Document
      - Of
      - Type+source
      - Exists
      - Within
  /api/role/{id}/attachdocument:
    put:
      summary: Attaches an existing document to a role
      description: Attaches an existing document to a role.
      operationId: Role_AttachDocumentByidBydocumentId
      x-api-path-slug: apiroleidattachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to attach
      - in: path
        name: id
        description: The id of the role to attach the document to
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Existing
      - Document
      - To
      - Role
  /api/role/{id}/detachdocument:
    put:
      summary: Detaches a document from a role
      description: Detaches a document from a role.
      operationId: Role_DetachDocumentByidBydocumentId
      x-api-path-slug: apiroleiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the role to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Role
  /api/role/{id}/uploadandattachdocument:
    post:
      summary: Allows you to upload a document and attach it directly to a role.
      description: Allows you to upload a document and attach it directly to a role..
      operationId: Role_UploadAndAttachDocumentByidBydocumentDetailsContract
      x-api-path-slug: apiroleiduploadandattachdocument-post
      parameters:
      - in: body
        name: documentDetailsContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Upload
      - Document
      - Attach
      - It
      - Directly
      - To
      - Role
  /api/role/{id}/attachexternaldocument:
    post:
      summary: Attaches an externally hosted document to a role
      description: Attaches an externally hosted document to a role.
      operationId: Role_AttachExternalDocumentByidBydocumentDetails
      x-api-path-slug: apiroleidattachexternaldocument-post
      parameters:
      - in: body
        name: documentDetails
        description: Details of the document to associate
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The role Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Externally
      - Hosted
      - Document
      - To
      - Role
  /api/roomdescription/{id}/attachexternaldocumenttoroom:
    put:
      summary: Attaches an externally hosted document to a room within a room description.
      description: Attaches an externally hosted document to a room within a room
        description..
      operationId: RoomDescription_AttachExternalDocumentToRoomByidByexternalDocumentByroomId
      x-api-path-slug: apiroomdescriptionidattachexternaldocumenttoroom-put
      parameters:
      - in: body
        name: externalDocument
        description: Details of the external document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The RoomDescriptionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The room identifier
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Externally
      - Hosted
      - Document
      - To
      - Room
      - Within
      - Room
      - Description
  /api/roomdescription/{id}/uploadandattachdocumenttoroom:
    put:
      summary: Uploads and attaches a document to room description room - the new
        document is appended to the current list.
      description: Uploads and attaches a document to room description room - the
        new document is appended to the current list..
      operationId: RoomDescription_UploadAndAttachDocumentToRoomByidByroomIdBydocumentDetails
      x-api-path-slug: apiroomdescriptioniduploadandattachdocumenttoroom-put
      parameters:
      - in: body
        name: documentDetails
        description: Details about the document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The room description Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The roomId
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Room
      - Description
      - Room
      - '-'
      - New
      - Document
      - Is
      - Appended
      - To
      - Current
      - List
  /api/roomdescription/{id}/attachdocumentoroom:
    put:
      summary: Attaches the document to room.
      description: Attaches the document to room..
      operationId: RoomDescription_AttachDocumentToRoomByidBydocumentIdByroomIdByinsertAtIndex
      x-api-path-slug: apiroomdescriptionidattachdocumentoroom-put
      parameters:
      - in: query
        name: documentId
        description: The document identifier
      - in: path
        name: id
        description: The identifier
      - in: query
        name: insertAtIndex
        description: Index of the insert at
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The room identifier
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Document
      - To
      - Room
  /api/roomdescription/{id}/detachdocumentfromroom:
    put:
      summary: Detaches a document from a room description room.
      description: Detaches a document from a room description room..
      operationId: RoomDescription_DetachDocumentFromRoomByidBydocumentIdByroomId
      x-api-path-slug: apiroomdescriptioniddetachdocumentfromroom-put
      parameters:
      - in: query
        name: documentId
        description: The document Id
      - in: path
        name: id
        description: The room description Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The room Id
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Room
      - Description
      - Room
  /api/stationary/html/{brandId}:
    get:
      summary: "Does a simple merge of the selected envelopeTemplatePack using the
        data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document."
      description: "Does a simple merge of the selected envelopetemplatepack using
        the data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document.."
      operationId: Stationary_HtmlStationaryBybrandId
      x-api-path-slug: apistationaryhtmlbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Does
      - Simple
      - Merge
      - Of
      - Selected
      - EnvelopeTemplatePack
      - Using
      - Data
      - "Supplied\r\nWill"
      - Only
      - Use
      - Certain
      - Merge
      - Functions
      - ""
      - Correspondence
      - Can
      - Only
      - Contain
      - Envelope
      - Envelope
      - Can
      - Only
      - Contain
      - Document
  /api/stationary/sms/{brandId}:
    get:
      summary: "Does a simple merge of the selected envelopeTemplatePack using the
        data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document."
      description: "Does a simple merge of the selected envelopetemplatepack using
        the data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document.."
      operationId: Stationary_SmsStationaryBybrandId
      x-api-path-slug: apistationarysmsbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Does
      - Simple
      - Merge
      - Of
      - Selected
      - EnvelopeTemplatePack
      - Using
      - Data
      - "Supplied\r\nWill"
      - Only
      - Use
      - Certain
      - Merge
      - Functions
      - ""
      - Correspondence
      - Can
      - Only
      - Contain
      - Envelope
      - Envelope
      - Can
      - Only
      - Contain
      - Document
  /api/tenancy/{id}/detachdocument:
    put:
      summary: Detaches a document from a tenancy role
      description: Detaches a document from a tenancy role.
      operationId: Tenancy_DetachDocumentByidBydocumentId
      x-api-path-slug: apitenancyiddetachdocument-put
      parameters:
      - in: query
        name: documentId
        description: The id of the document to detach
      - in: path
        name: id
        description: The id of the role to detach the document from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detaches
      - Document
      - From
      - Tenancy
      - Role
  /api/admin/system/updateDocumentGenerationMetadataFile:
    post:
      summary: Updates the metadata for document generation merge fields
      description: Updates the metadata for document generation merge fields.
      operationId: System_UpdateDocumentGenerationMetadataFile
      x-api-path-slug: apiadminsystemupdatedocumentgenerationmetadatafile-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Metadatadocument
      - Generation
      - Merge
      - Fields
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