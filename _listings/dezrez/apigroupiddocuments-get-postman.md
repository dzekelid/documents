{
  "info": {
    "name": "Dezrez Get a list of documents belonging to a group",
    "_postman_id": "14fde95c-0735-4529-8bf7-f33cd547cb2b",
    "description": "Get a list of documents belonging to a group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Documents",
      "item": [
        {
          "id": "c41d5459-6275-4cf4-83dc-0a6af1284abd",
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
              "id": "761aa403-015f-4250-b974-c4217947f06f"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "67425e9d-0f66-439d-b001-644c6bf64353",
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
              "id": "4d9a2813-25b4-4b95-8ad5-839d27ef5fd6"
            }
          ]
        }
      ]
    }
  ]
}