swagger: "2.0"
x-collection-name: SAP
x-complete: 1
info:
  title: SAP Translation Hub
  description: to-provide-users-of-software-in-a-global-market-with-texts-in-their-own-language-translations-are-required--sap-translation-hub-enables-you-to-draw-on-saps-translation-experience-across-multiple-products-and-languages-to-propose-translations-for-short-texts-
  contact:
    name: SAP Translation Hub team
    email: translationhub@sap.com
  version: 1.0.0
host: sandbox.api.sap.com
basePath: /translationhub/api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborationRooms/{collaborationRoomId}/documents:
    get:
      summary: Retrieves documents in a collaboration room
      description: Retrieves the information of all documents in a collaboration room,
        such as design files and specifications.
      operationId: retrieves-the-information-of-all-documents-in-a-collaboration-room-such-as-design-files-and-specific
      x-api-path-slug: collaborationroomscollaborationroomiddocuments-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Documents
      - In
      - Collaboration
      - Room
  /collaborationRooms/{collaborationRoomId}/documents/{fileId}:
    get:
      summary: Retrieves a document
      description: Retrieves the information of a document by its ID.
      operationId: retrieves-the-information-of-a-document-by-its-id
      x-api-path-slug: collaborationroomscollaborationroomiddocumentsfileid-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: fileId
        description: The ID of a file
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - Document
    delete:
      summary: Deletes a document
      description: "Deletes a document.  \nThe login technical user must be the one
        who uploaded the document."
      operationId: deletes-a-document--the-login-technical-user-must-be-the-one-who-uploaded-the-document
      x-api-path-slug: collaborationroomscollaborationroomiddocumentsfileid-delete
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: fileId
        description: The ID of a file
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Document