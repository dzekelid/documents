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
  /resellernotify/unregister:
    post:
      summary: Unregister Reseller
      description: Unregisters a Reseller for receiving notifications
      operationId: reseller.resellernotify.unregister
      parameters:
      - in: query
        name: serviceAccountEmailAddress
        description: The service account which owns the Cloud-PubSub topic
      responses:
        200:
          description: OK
      tags:
      - register
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