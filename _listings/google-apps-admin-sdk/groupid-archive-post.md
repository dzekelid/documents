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
  /{groupId}/archive:
    post:
      summary: Archive Mail
      description: Inserts a new mail into the archive of the Google group
      operationId: groupsmigration.archive.insert
      parameters:
      - in: path
        name: groupId
        description: The group ID
      responses:
        200:
          description: OK
      tags:
      - archive
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