---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 0
info:
  title: AWS CloudSearch Index Documents
  version: 1.0.0
  description: Tells the search domain to start indexing its documents using the latest
    indexing options.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=IndexDocuments:
    get:
      summary: Index Documents
      description: Tells the search domain to start indexing its documents using the
        latest indexing options.
      operationId: IndexDocuments
      x-api-path-slug: actionindexdocuments-get
      parameters:
      - in: query
        name: DomainName
        description: A string that represents the name of a domain
        type: string
      responses:
        200:
          description: OK
      tags:
      - Index Documents
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