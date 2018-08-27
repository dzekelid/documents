{
  "info": {
    "name": "Dezrez Get a list of documents belonging to a group",
    "_postman_id": "78ee45d0-1d86-4733-8b14-f1c5351bb64b",
    "description": "Get a list of documents belonging to a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Documents",
      "item": [
        {
          "id": "f1b8a684-1279-4564-92a7-f589ecc27ca0",
          "name": "Document_GetByids",
          "request": {
            "url": "http://api.dezrez.com/api/Document?ids=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get documents by their ids."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46478927-ff49-46e8-bb78-fffbd0661bc3"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "775f83e6-2ec1-4e7e-ba7b-d39e9a63f33d",
          "name": "Group_DocumentsByidBysubTypesBypageSizeBypageNumberBytypeByorderDesc",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/group/:id/documents"
              ],
              "query": [
                {
                  "key": "orderDesc",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "subTypes",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of documents belonging to a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "783692e9-0873-4daf-9a70-1bf82a0a0fa2"
            }
          ]
        },
        {
          "id": "832924d9-a6f3-4a16-951b-0b24fb937ac6",
          "name": "Group_OffersMadeByidBypageSizeBypageNumber",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/group/:id/offers/made"
              ],
              "query": [
                {
                  "key": "pageNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of documents belonging to a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2efbad9d-45fa-4d4a-a386-b2973f37397c"
            }
          ]
        }
      ]
    }
  ]
}