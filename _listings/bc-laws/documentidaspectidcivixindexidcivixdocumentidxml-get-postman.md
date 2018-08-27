{
  "info": {
    "name": "BC Laws Retrieves a specific document from the BCLaws legislative repository (XML format)",
    "_postman_id": "944dd38a-0dfe-41ec-97c3-e5969ff18302",
    "description": "The /document API allows you to retrieve actual documents from the BCLaws legislative repository. To retrieve a document from the repository you need the aspect identifier and two other specific pieces of information about the document: the index identifier and the document identifier. These unique identifiers can be retrieved from the /content API.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Content",
      "item": [
        {
          "id": "16d417a6-a62c-4c1e-93cd-51f2a4f10411",
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
              "id": "0baaa1ce-06c5-4353-9773-7494888444e5"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "59c06e03-107c-4d45-b1fe-e88db9920858",
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
              "id": "73c02b02-9429-4510-ba09-0bb90369a5c8"
            }
          ]
        },
        {
          "id": "cb5f4118-d958-47ad-96b1-a3e6524ffe13",
          "name": "getDocumentAspectCivixindexCivixdocumentSearchSearchstring",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "document/id/:aspectId/:civixIndexId/:civixDocumentId/search/:searchString"
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
                },
                {
                  "id": "searchString",
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
              "id": "6830b15f-445b-4f6b-a729-219dc1bc5054"
            }
          ]
        },
        {
          "id": "03b46e30-7002-4214-94f0-fb0b173952f4",
          "name": "getDocumentAspectCivixindexCivixdocumentXml",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "document/id/:aspectId/:civixIndexId/:civixDocumentId/xml"
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
              "id": "d0580493-0fab-463f-a792-c678ac8de84e"
            }
          ]
        }
      ]
    }
  ]
}