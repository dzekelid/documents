{
  "info": {
    "name": "AWS CloudSearch Index Documents",
    "_postman_id": "a953752f-54dd-4ec8-b8a3-1fba29f8bcc0",
    "description": "Tells the search domain to start indexing its documents using the latest indexing options.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "0d1682b1-8787-4de7-ba96-3488871c7a38",
          "name": "AddTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?Base=Base&InternalException=InternalException&LimitExceededException=LimitExceededException&ValidationException=ValidationException",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches resource tags to an\n Amazon CloudSearch domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf05d853-fd11-4a3f-a1da-09ca1608ceaa"
            }
          ]
        }
      ]
    },
    {
      "name": "Suggesters",
      "item": [
        {
          "id": "847d8612-3c74-4944-94fe-a22a469c13ed",
          "name": "BuildSuggesters",
          "request": {
            "url": "http://example.com/api/?Action=BuildSuggesters?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Indexes the search suggestions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfa4eb60-413c-4d16-9cea-992613a47ca9"
            }
          ]
        },
        {
          "id": "2e477af0-8c0d-4f21-a386-d2c005ddde1b",
          "name": "DefineSuggester",
          "request": {
            "url": "http://example.com/api/?Action=DefineSuggester?DomainName=DomainName&Suggester=Suggester",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures a suggester for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18ba01b7-2cf9-48fd-b465-4e05019b8e3e"
            }
          ]
        },
        {
          "id": "c179c29d-ab17-4000-ac1a-b619a6040ff5",
          "name": "DeleteSuggester",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSuggester?DomainName=DomainName&SuggesterName=SuggesterName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a suggester."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9be8afa6-263d-47c3-aa09-f9958fabb799"
            }
          ]
        },
        {
          "id": "3944446a-75be-4733-a173-2cfb8ebd9c06",
          "name": "DescribeSuggesters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSuggesters?Deployed=Deployed&DomainName=DomainName&SuggesterNames.member.N=SuggesterNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the suggesters configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d57461a1-bd86-472d-bbdb-102b695f2d1a"
            }
          ]
        }
      ]
    },
    {
      "name": "Domains",
      "item": [
        {
          "id": "3772dafa-8f63-45ad-8e68-f53aa44f6e8c",
          "name": "CreateDomain",
          "request": {
            "url": "http://example.com/api/?Action=CreateDomain?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91923165-e425-471a-b036-426265bbadb4"
            }
          ]
        },
        {
          "id": "72c99d61-0599-4631-b3d0-840c3fd62afd",
          "name": "DeleteDomain",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDomain?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Permanently deletes a search domain and all of its data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fdd79ac-4e46-41f6-88d3-53ce89c6351e"
            }
          ]
        },
        {
          "id": "bc042042-9473-4e93-8729-7a1983f00be7",
          "name": "DescribeDomains",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDomains?DomainNames.member.N=DomainNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the search domains owned by this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee920070-eb9f-49d3-9697-cfad832c3a2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Analysis Scheme",
      "item": [
        {
          "id": "3f0fb3b9-fed8-4df7-b19f-8baeb34465fd",
          "name": "DefineAnalysisScheme",
          "request": {
            "url": "http://example.com/api/?Action=DefineAnalysisScheme?AnalysisScheme=AnalysisScheme&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an analysis scheme that can be applied to a text or text-array field to define language-specific text processing options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "550c9336-22c4-408e-854c-ca3a4e15346e"
            }
          ]
        },
        {
          "id": "7ae2ce79-c70e-4f9a-a645-65928c019dc8",
          "name": "DeleteAnalysisScheme",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAnalysisScheme?AnalysisSchemeName=AnalysisSchemeName&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an analysis scheme."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f1d6f79-bd16-43b4-92da-438e859ea43b"
            }
          ]
        },
        {
          "id": "0db2d4fa-88fc-4ff4-bed6-065e48f88428",
          "name": "DescribeAnalysisSchemes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAnalysisSchemes?AnalysisSchemeNames.member.N=AnalysisSchemeNames.member.N&Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the analysis schemes configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "49e7f85f-1d3b-47e2-bb26-d250733eb803"
            }
          ]
        }
      ]
    },
    {
      "name": "Expressions",
      "item": [
        {
          "id": "be26be16-9bef-4eb4-947d-872018beb083",
          "name": "DefineExpression",
          "request": {
            "url": "http://example.com/api/?Action=DefineExpression?DomainName=DomainName&Expression=Expression",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an Expression  for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acf90cc0-c354-4708-8ada-5b9ef4c24f44"
            }
          ]
        },
        {
          "id": "0b59ba79-470f-48d3-8e41-769cb8aec5f8",
          "name": "DeleteExpression",
          "request": {
            "url": "http://example.com/api/?Action=DeleteExpression?DomainName=DomainName&ExpressionName=ExpressionName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an \n  Expression\n  from the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a3a5b7f-e4cf-4047-aef4-e46049101a36"
            }
          ]
        },
        {
          "id": "17311a2d-371a-45ce-bf7c-f232fbcf9c27",
          "name": "DescribeExpressions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeExpressions?Deployed=Deployed&DomainName=DomainName&ExpressionNames.member.N=ExpressionNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the expressions configured for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66197f77-6606-42c2-b70a-74363ce00e8c"
            }
          ]
        }
      ]
    },
    {
      "name": "Index Fields",
      "item": [
        {
          "id": "f203a52f-f7a0-4386-8b07-3562640a53fb",
          "name": "DefineIndexField",
          "request": {
            "url": "http://example.com/api/?Action=DefineIndexField?DomainName=DomainName&IndexField=IndexField",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures an ndexField  for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3645f860-0ca8-410c-b437-1165ba774082"
            }
          ]
        },
        {
          "id": "2a938a48-4160-4722-a819-a07fb9b9bb48",
          "name": "DeleteIndexField",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIndexField?DomainName=DomainName&IndexFieldName=IndexFieldName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes an \n  IndexField\n  from the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e760fc4-9f11-4b98-b900-bd567c6db772"
            }
          ]
        },
        {
          "id": "4d22a8b3-9853-40d3-b291-0518f20a49fa",
          "name": "DescribeIndexFields",
          "request": {
            "url": "http://example.com/api/?Action=DescribeIndexFields?Deployed=Deployed&DomainName=DomainName&FieldNames.member.N=FieldNames.member.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the index fields configured for the search domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c23d12f0-5d96-4d39-80f3-e0ca333bcf6e"
            }
          ]
        }
      ]
    },
    {
      "name": "Availability Options",
      "item": [
        {
          "id": "a4f72bfe-d0cd-4e48-ac11-35b519aaa11a",
          "name": "DescribeAvailabilityOptions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailabilityOptions?Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the availability options configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4e03670-821c-4341-8ad0-7d84cf8ddf06"
            }
          ]
        }
      ]
    },
    {
      "name": "Scaling Parameters",
      "item": [
        {
          "id": "062cb58c-5928-49a9-af73-253865181007",
          "name": "DescribeScalingParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeScalingParameters?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the scaling parameters configured for a domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3bca5182-f120-482e-8683-bed4233618bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Service Access Policies",
      "item": [
        {
          "id": "340e1f92-786b-40b5-8b99-3d6640f0f9d7",
          "name": "DescribeServiceAccessPolicies",
          "request": {
            "url": "http://example.com/api/?Action=DescribeServiceAccessPolicies?Deployed=Deployed&DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about the access policies that control access to the domain's document and search endpoints."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57691fe2-2a3f-4251-88ab-1e624a16f273"
            }
          ]
        }
      ]
    },
    {
      "name": "Index Documents",
      "item": [
        {
          "id": "e63a77a4-a656-48e0-938b-6033e94eb93e",
          "name": "IndexDocuments",
          "request": {
            "url": "http://example.com/api/?Action=IndexDocuments?DomainName=DomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Tells the search domain to start indexing its documents using the latest indexing options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "faa47540-cdce-4072-a859-b17b9aae47b7"
            }
          ]
        }
      ]
    }
  ]
}