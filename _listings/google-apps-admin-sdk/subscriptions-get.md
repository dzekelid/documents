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
  /subscriptions:
    get:
      summary: List Subscriptions
      description: List of subscriptions managed by the reseller
      operationId: reseller.subscriptions.list
      parameters:
      - in: query
        name: customerAuthToken
        description: The customerAuthToken query string is required when creating
          a resold account that transfers a direct customer's subscription or transfers
          another reseller customer's subscription to your reseller management
      - in: query
        name: customerId
        description: Either the customer's primary domain name or the customer's unique
          identifier
      - in: query
        name: customerNamePrefix
        description: When retrieving all of your subscriptions and filtering for specific
          customers, you can enter a prefix for a customer name
      - in: query
        name: maxResults
        description: When retrieving a large list, the maxResults is the maximum number
          of results per page
      - in: query
        name: pageToken
        description: Token to specify next page in the list
      responses:
        200:
          description: OK
      tags:
      - subscription
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