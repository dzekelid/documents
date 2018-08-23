{
  "info": {
    "name": "Dezrez Get documents by their ids",
    "_postman_id": "14e49f89-b734-4cf5-957d-7c251e2dd868",
    "description": "Get documents by their ids.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Documents",
      "item": [
        {
          "id": "772760b2-3f72-4831-81c5-5202038d2260",
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
              "id": "ed1492e6-db58-4023-a1f2-5b9b1a254dd3"
            }
          ]
        }
      ]
    }
  ]
}