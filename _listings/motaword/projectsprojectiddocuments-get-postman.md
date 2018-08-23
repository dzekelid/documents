{
  "info": {
    "name": "Mota Word Get a list of documents",
    "_postman_id": "412cb034-348e-42fd-9be6-fe0d7bff6e0b",
    "description": "Get a list of documents.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "f9a2e0a1-c4ca-4879-ba9e-a4455c20321d",
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
              "id": "d435727c-9884-4372-b46d-7d2fdbf306eb"
            }
          ]
        }
      ]
    }
  ]
}