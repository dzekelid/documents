{
  "info": {
    "name": "BC Laws Retrieves a specific document from the BCLaws legislative repository (HTML format)",
    "_postman_id": "befbf1f5-0e97-4ec1-a9e9-f8befc272fdc",
    "description": "The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Content",
      "item": [
        {
          "id": "c477b057-9b5e-4f5f-8b16-b3c70cdc5dfb",
          "name": "getContentAspectCivixdocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "content/:aspectId/:civixDocumentId"
              ],
              "variable": [
                {
                  "id": "aspectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixDocumentId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the metadata available for the specified index or directory from the BCLaws legislative respository"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b433793-3525-48e5-9e28-0df86fdd544f"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "46240555-a00a-434d-84f5-aeb6ddc0b1e6",
          "name": "getDocumentAspectCivixindexCivixdocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "document/id/:aspectId/:civixIndexId/:civixDocumentId"
              ],
              "variable": [
                {
                  "id": "aspectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixDocumentId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixIndexId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cedbed52-fb4c-4e26-a657-850b300895b2"
            }
          ]
        }
      ]
    }
  ]
}