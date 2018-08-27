---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/{requestId}/condition/{condition}/documents:
    get:
      summary: Get Request Requestid Condition Condition Documents
      description: Get request requestid condition condition documents.
      operationId: getApiV1RequestRequestConditionConditionDocuments
      x-api-path-slug: apiv1requestrequestidconditionconditiondocuments-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: condition
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Condition
      - Documents
    post:
      summary: Post Request Requestid Condition Condition Documents
      description: Post request requestid condition condition documents.
      operationId: postApiV1RequestRequestConditionConditionDocuments
      x-api-path-slug: apiv1requestrequestidconditionconditiondocuments-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Condition
      - Condition
      - Documents
---