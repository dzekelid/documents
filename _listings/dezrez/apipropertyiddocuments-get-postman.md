{
  "info": {
    "name": "Dezrez Get the documents of a property by the property Id",
    "_postman_id": "944dc023-d6e3-47bc-b33b-41c2fc2b2e88",
    "description": "Get the documents of a property by the property id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Documents",
      "item": [
        {
          "id": "ed325922-378c-4225-b705-fae1655b920e",
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
              "id": "531ddab1-dae8-49bf-959d-5146ec6f9b6e"
            }
          ]
        },
        {
          "id": "e4148cf5-b95a-4ec8-a9d7-9e4154c531d1",
          "name": "Property_DocumentsByidBysubTypesBypageSizeBypageNumberBytype",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/:id/documents"
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
            "description": "Get the documents of a property by the property id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ceef17b-b61d-4df0-9013-5779963eedc8"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "82521ed3-8a4e-4ff8-8cf0-1e121a0ba6a2",
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
              "id": "c2129922-e4ea-44a3-b101-9fe491e3aa21"
            }
          ]
        },
        {
          "id": "125c47b1-0d04-495d-a8e8-8cd561a5d386",
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
              "id": "a088b1a8-7d88-4311-a492-9b95c7382e70"
            }
          ]
        },
        {
          "id": "fc058209-2bc9-4ba7-966e-c34e877abb1a",
          "name": "Group_OffersReceivedByidBypageSizeBypageNumber",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/group/:id/offers/received"
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
              "id": "774db4d9-79d4-4425-ab78-e44cbfd06c36"
            }
          ]
        }
      ]
    }
  ]
}