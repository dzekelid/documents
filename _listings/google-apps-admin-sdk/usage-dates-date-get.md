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
  /usage/dates/{date}:
    get:
      summary: Get Report by Date
      description: Retrieves a report which is a collection of properties / statistics
        for a specific customer
      operationId: reports.customerUsageReports.get
      parameters:
      - in: query
        name: customerId
        description: Represents the customer for which the data is to be fetched
      - in: path
        name: date
        description: Represents the date in yyyy-mm-dd format for which the data is
          to be fetched
      - in: query
        name: pageToken
        description: Token to specify next page
      - in: query
        name: parameters
        description: Represents the application name, parameter name pairs to fetch
          in csv as app_name1:param_name1, app_name2:param_name2
      responses:
        200:
          description: OK
      tags:
      - report
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