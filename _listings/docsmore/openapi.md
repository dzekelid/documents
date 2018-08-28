swagger: "2.0"
x-collection-name: Docsmore
x-complete: 1
info:
  title: Docsmore API 2.1
  description: alt-texthttpswww-docsmore-comwpcontentuploads201802docsmoreapi-png-titleh3create-a-developer-account-at-docsmore-io-and-start-unleashing-the-power-of-docsmore-into-your-own-applications--to-make-it-easier-we-have-provided-client-libraries-and-sdk-in-several-languages-for-you-to-get-started-and-hit-the-ground-running-in-no-time-h3brbrh4note-if-you-dont-see-api-setting-under-top-right-menu-that-means-you-will-need-to-be-a-developer-account--please-contact-supportdocsmore-com-and-a-customer-service-expert-will-switch-your-account-to-developer-account--h4brbrh5just-head-over-to-httpsdocsmore-io-and-sign-up-for-your-30-days-trial-h5
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/dmcatalogue:
    post:
      summary: Fetch All Documents from Your Team Catalogue
      description: By design, the authenticated user can only view the files that
        are either created by them or shared with them. Make sure user has at least
        read permission to view the catalogue.
      operationId: ApiDmcataloguePost
      x-api-path-slug: apidmcatalogue-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: items
      - in: query
        name: page
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - ""
      - Documents
      - From
      - Your
      - Team
      - Catalogue
  /api/clientdocs/getrawdata/:authToken/:documentKey:
    get:
      summary: Get Raw Data For A Given Document
      description: |-
        This API call gets you underlying raw data of the document. All you need to do is supply Auth token and Document Key as part of the call.

        Document Key can be obtained from "Document Gallery" Page and Clicking on the sub-menu of the desired document.

        As a response object, jsondata and metadata information is passed. Jsondata is basically raw data and metadata is data columns information.
      operationId: ApiClientdocsGetrawdataAuthTokenDocumentKeyGet
      x-api-path-slug: apiclientdocsgetrawdataauthtokendocumentkey-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: authToken
      - in: header
        name: Content-Type
      - in: query
        name: documentKey
      responses:
        200:
          description: OK
      tags:
      - Raw
      - Data
      - Given
      - Document
  /api/dmcatalogue/:id:
    post:
      summary: Fetch Single Document
      description: Fetch single document.
      operationId: ApiDmcatalogueIdPost
      x-api-path-slug: apidmcatalogueid-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Single
      - Document
  /api/docflow/getdocflows:
    get:
      summary: Get All Document Flows
      description: Get all document flows.
      operationId: ApiDocflowGetdocflowsGet
      x-api-path-slug: apidocflowgetdocflows-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Document
      - Flows
  /api/docflowtracks/flowtrackviaapi:
    post:
      summary: Get Workflow Link For Flow Track
      description: |-
        In Docsmore space, Flow Track means all the client documents generated using one of the Document Flow. In other words, it is an instance of Document FLow. The other thing to notice here is payload information is remarkably similar to general "Workflow" of a Single Document.

        When you initiate this API call, you are basically setting up a new instance of Workflow and in turn getting workflow link of the starting document in the workflow.

        If "flowtrackid" value is "new", then new flowtrack will be created. If flowtrackid has a value of actual flowtrackid then link will be provided to access read-only view of document flowtrack
      operationId: ApiDocflowtracksFlowtrackviaapiPost
      x-api-path-slug: apidocflowtracksflowtrackviaapi-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Link
      - Flow
      - Track
  /getclientdocs:
    post:
      summary: Get List of Client Documents By Document ID
      description: In order to export as PDf, you will need to have client document
        ID available for that specific document you are looking to download.
      operationId: GetclientdocsPost
      x-api-path-slug: getclientdocs-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Client
      - Documents
      - Document
      - ID