{
  "info": {
    "name": "Mota Word Upload a new document",
    "_postman_id": "3ffdd9b4-27fa-4b9d-ac85-2c1b64fdb9f8",
    "description": "Upload a new document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "a433a6dc-89ee-4dff-b6d0-384b5e550650",
          "name": "getDocuments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2a892c0d-758e-49d0-81ac-dd3ea5592aad"
            }
          ]
        },
        {
          "id": "e8355514-998b-4754-8fac-b28857972417",
          "name": "createDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.motaword.com",
              "path": [
                "projects/:projectId/documents"
              ],
              "variable": [
                {
                  "id": "projectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "documents",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "You can add as many files as you want in documents[] parameter"
                },
                {
                  "key": "schemes",
                  "value": "[{}]",
                  "disabled": false,
                  "description": "JSON string"
                }
              ]
            },
            "description": "Upload a new document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1117cba-6d48-4cdb-88df-a857c6445b32"
            }
          ]
        }
      ]
    }
  ]
}