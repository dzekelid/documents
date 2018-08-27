{
  "info": {
    "name": "Dezrez Get a list of documents belonging to a role",
    "_postman_id": "227c924a-13c2-4740-bbf2-82c29107b65b",
    "description": "Get a list of documents belonging to a role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Documents",
      "item": [
        {
          "id": "33559344-022f-430d-8176-ba2139c46eb8",
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
              "id": "c3ce1aa0-21e7-44ee-808f-f044b65ded8d"
            }
          ]
        },
        {
          "id": "434243cd-7dba-4d8d-a376-cd58a8885444",
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
              "id": "490f9540-e53e-4301-83ec-58206c3412b6"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "b055ed47-cfa5-4c5a-acc5-3443d8de4337",
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
              "id": "778a28af-13b7-4af3-8315-2946aa575623"
            }
          ]
        },
        {
          "id": "8dfbb610-ebb2-4e15-859d-8e2cf57cfed0",
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
              "id": "d7415a14-140e-40a0-bee9-82582544a0a0"
            }
          ]
        },
        {
          "id": "d2d84653-093b-4f25-9ea2-226de0e99af0",
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
              "id": "d4054a8e-d7ea-4133-83f3-9618d95c6c49"
            }
          ]
        },
        {
          "id": "37a03071-5ac1-4a48-b42f-081da82cf418",
          "name": "Role_DocumentsByidBysubTypesBypageSizeBypageNumberBytypeByorderDesc",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/role/:id/documents"
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
            "description": "Get a list of documents belonging to a role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9ace3a8-a881-4fb2-a79a-080212ed761d"
            }
          ]
        }
      ]
    }
  ]
}