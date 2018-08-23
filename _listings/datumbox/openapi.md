---
swagger: "2.0"
x-collection-name: Datumbox
x-complete: 1
info:
  title: DatumBox
  description: datumbox-offers-a-machine-learning-platform-composed-of-14-classifiers-and-natural-language-processing-functions--functions-include-sentiment-analysis-topic-classification-readability-assessment-language-detection-and-much-more-
  version: 1.0.0
host: api.datumbox.com
basePath: 1.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /DocumentSimilarity.json:
    post:
      summary: Estimates the similarity between 2 Documents
      description: The Document Similarity function estimates the degree of similarity
        between two documents. It can be used to detect duplicate webpages or detect
        plagiarism.
      operationId: DocumentSimilarity
      x-api-path-slug: documentsimilarity-json-post
      parameters:
      - in: formData
        name: copy
        description: The second text
      - in: formData
        name: original
        description: The first text
      responses:
        200:
          description: OK
      tags:
      - DocumentsSimilarity
---