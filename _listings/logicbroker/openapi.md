swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 1
info:
  title: CommerceAPI
  version: 1.0.0
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Document/Script/{ScriptName}:
    get:
      summary: Execute custom handler.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Document_GetCustomScript
      x-api-path-slug: apiv1documentscriptscriptname-get
      parameters:
      - in: path
        name: ScriptName
        description: The custom script name
      responses:
        200:
          description: OK
      tags:
      - Execute
      - Custom
      - Handler
    post:
      summary: Execute custom handler.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Document_PostCustomScript
      x-api-path-slug: apiv1documentscriptscriptname-post
      parameters:
      - in: path
        name: ScriptName
        description: The custom script name
      responses:
        200:
          description: OK
      tags:
      - Execute
      - Custom
      - Handler
    options:
      summary: Execute custom handler.
      description: Request rate limited to 2 requests per second with bursts up to
        25 requests.
      operationId: Document_OptionsCustomScript
      x-api-path-slug: apiv1documentscriptscriptname-options
      parameters:
      - in: path
        name: ScriptName
        description: The custom script name
      responses:
        200:
          description: OK
      tags:
      - Execute
      - Custom
      - Handler
  /api/v1/Statuses/{documentType}:
    get:
      summary: Get configured document statuses for each document
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Status_GetDocumentStatusesByType
      x-api-path-slug: apiv1statusesdocumenttype-get
      parameters:
      - in: path
        name: documentType
        description: Document type
      responses:
        200:
          description: OK
      tags:
      - Configured
      - Document
      - Statuseseach
      - Document
  /api/v1/Statuses:
    get:
      summary: Get configured document statuses for each document
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Status_GetDocumentStatuses
      x-api-path-slug: apiv1statuses-get
      responses:
        200:
          description: OK
      tags:
      - Configured
      - Document
      - Statuseseach
      - Document