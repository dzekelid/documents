{
  "info": {
    "name": "Plentymarkets Get a temporary url for a single document",
    "_postman_id": "378f3b9d-a796-41d4-9295-37a6d217d18d",
    "description": "Get a temporary url for a single document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Single",
      "item": [
        {
          "id": "cbb99ff7-3d16-4098-afc8-27cf0a4e32fb",
          "name": "getRestAccountsContactsContactDocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/document"
              ],
              "query": [
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a single storage object from contact documents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc68f992-e49d-4d44-9371-f3e61a7c82f3"
            }
          ]
        }
      ]
    },
    {
      "name": "Temporary",
      "item": [
        {
          "id": "6a15a15c-7eee-449f-86c1-35f4e14bd130",
          "name": "getRestAccountsContactsContactDocumentUrl",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/:contactId/document/url"
              ],
              "query": [
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "contactId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a temporary url for a single document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ea63571-1c3a-46b0-9e47-e14fa113fe09"
            }
          ]
        }
      ]
    }
  ]
}