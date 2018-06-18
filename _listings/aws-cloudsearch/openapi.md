---
swagger: "2.0"
x-collection-name: AWS CloudSearch
x-complete: 1
info:
  title: AWS CloudSearch
  version: 1.0.0
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
---