{
  "info": {
    "name": "Datumbox Estimates the similarity between 2 Documents",
    "_postman_id": "0a8da714-f9ad-4b57-945d-7920caa37a79",
    "description": "The Document Similarity function estimates the degree of similarity between two documents. It can be used to detect duplicate webpages or detect plagiarism.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Adult Content",
      "item": [
        {
          "id": "d9f2ecde-e2f8-4423-90ed-d973a58dbae1",
          "name": "AdultContentDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/AdultContentDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Adult Content Detection function classifies the documents as adult or noadult based on their context. It can be used to detect whether a document contains content unsuitable for minors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c68f7de-202e-4028-96d3-bc3429a0a071"
            }
          ]
        }
      ]
    },
    {
      "name": "Commercial",
      "item": [
        {
          "id": "3ccc4cc6-812c-4a0b-8fdc-6ad2c24678a2",
          "name": "CommercialDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/CommercialDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Commercial Detection function labels the documents as commercial or non-commercial based on their keywords and expressions. It can be used to detect whether a website is commercial or not."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "547ab3ee-2477-4251-b9ec-73d932bb554c"
            }
          ]
        }
      ]
    },
    {
      "name": "DocumentsSimilarity",
      "item": [
        {
          "id": "0774b901-9202-4a0a-b014-9a11f3a97ea2",
          "name": "DocumentSimilarity",
          "request": {
            "url": "http://api.datumbox.com/1.0/DocumentSimilarity.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "copy",
                  "value": "{}",
                  "disabled": false,
                  "description": "The second text"
                },
                {
                  "key": "original",
                  "value": "{}",
                  "disabled": false,
                  "description": "The first text"
                }
              ]
            },
            "description": "The Document Similarity function estimates the degree of similarity between two documents. It can be used to detect duplicate webpages or detect plagiarism."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc3407ae-2be6-4e09-9c9c-741c5edd7b84"
            }
          ]
        }
      ]
    }
  ]
}