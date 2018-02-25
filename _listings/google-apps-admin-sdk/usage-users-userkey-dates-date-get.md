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
  /usage/users/{userKey}/dates/{date}:
    get:
      summary: Get User Report by Date
      description: Retrieves a report which is a collection of properties / statistics
        for a set of users
      operationId: reports.userUsageReport.get
      parameters:
      - in: query
        name: customerId
        description: Represents the customer for which the data is to be fetched
      - in: path
        name: date
        description: Represents the date in yyyy-mm-dd format for which the data is
          to be fetched
      - in: query
        name: filters
        description: Represents the set of filters including parameter operator value
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: Token to specify next page
      - in: query
        name: parameters
        description: Represents the application name, parameter name pairs to fetch
          in csv as app_name1:param_name1, app_name2:param_name2
      - in: path
        name: userKey
        description: Represents the profile id or the user email for which the data
          should be filtered
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