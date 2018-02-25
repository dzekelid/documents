---
swagger: "2.0"
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{productId}/sku/{skuId}/user/{userId}:
    patch:
      summary: Update License
      description: Assign License
      operationId: licensing.licenseAssignments.patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: productId
        description: Name for product
      - in: path
        name: skuId
        description: Name for sku for which license would be revoked
      - in: path
        name: userId
        description: email id or unique Id of the user
      responses:
        200:
          description: OK
      tags:
      - license
definitions: []
x-collection-name: Google Apps Admin SDK
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