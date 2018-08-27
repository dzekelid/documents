{
  "info": {
    "name": "Amazon EC2 Systems Manager API Delete Document",
    "_postman_id": "f8a51cdc-2b33-4568-89bf-c5f890470919",
    "description": "Deletes the SSM document and all instance associations to the document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "a2a86327-9999-47ae-b3f7-024a5ea69299",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&ResourceType=ResourceType&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e9a9fdd1-1f1f-4b08-ae88-810e2294602a"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "f2ace88f-4a56-435b-a034-e1a388b9db1f",
          "name": "cancelCommand",
          "request": {
            "url": "http://example.com/api/?Action=CancelCommand?CommandId=CommandId&InstanceIds=InstanceIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attempts to cancel the command specified by the Command ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82028572-2b17-40e5-bbac-4d215a04547f"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "d243c70f-f602-45e3-9e92-b5c4bccdd9e4",
          "name": "createActivation",
          "request": {
            "url": "http://example.com/api/?Action=CreateActivation?DefaultInstanceName=DefaultInstanceName&Description=Description&ExpirationDate=ExpirationDate&IamRole=IamRole&RegistrationLimit=RegistrationLimit",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers your on-premises server or virtual machine with Amazon EC2 so that you can manage\n   these resources using Run Command."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ff158c5-c17c-4be8-9083-77d93f15cb07"
            }
          ]
        },
        {
          "id": "0c083134-0785-4b1b-9a1a-c46e01bfce62",
          "name": "deleteActivation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteActivation?ActivationId=ActivationId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an activation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c30293d-ad93-4ace-9ee7-91725da81ee1"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "617abc7d-ac5f-42d1-a1ac-2390f7663ebf",
          "name": "createAssociation",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociation?DocumentVersion=DocumentVersion&InstanceId=InstanceId&Name=Name&OutputLocation=OutputLocation&Parameters=Parameters&ScheduleExpression=ScheduleExpression&Targets=Targets",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d6173f7-25f5-4fd8-97ed-d044e76d5e63"
            }
          ]
        },
        {
          "id": "835da348-8558-4704-bf60-8c8427597fc7",
          "name": "createAssociationBatch",
          "request": {
            "url": "http://example.com/api/?Action=CreateAssociationBatch?Entries=Entries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates the specified SSM document with the specified instances or targets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50b57066-0f83-4a1f-94f7-f113a8b916d2"
            }
          ]
        },
        {
          "id": "0da9e003-e6a7-4585-80c3-1d6e5b7cf87e",
          "name": "deleteAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DeleteAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disassociates the specified SSM document from the specified instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c0ec200-e34f-4152-a402-a12b0a19a77e"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "b274e972-c151-44be-84c0-486c7a53b841",
          "name": "createDocument",
          "request": {
            "url": "http://example.com/api/?Action=CreateDocument?Content=Content&DocumentType=DocumentType&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b154de6-cd6e-426d-9b97-9b5080c00313"
            }
          ]
        },
        {
          "id": "2159e844-1439-4c81-9d19-2edbb58868d9",
          "name": "deleteDocument",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDocument?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the SSM document and all instance associations to the document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82fd393a-eb1d-4eda-b1ed-1ade14d94ef5"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "b8ca7ad3-ddd7-4beb-a0a8-cd9c74efbefb",
          "name": "createMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=CreateMaintenanceWindow?AllowUnassociatedTargets=AllowUnassociatedTargets&ClientToken=ClientToken&Cutoff=Cutoff&Duration=Duration&Name=Name&Schedule=Schedule",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cdd854e-3cfa-431f-8d07-333de653622e"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "f0ff619b-a79d-4cee-a1cd-fd3dac0073fe",
          "name": "createPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePatchBaseline?ApprovalRules=ApprovalRules&ApprovedPatches=ApprovedPatches&ClientToken=ClientToken&Description=Description&GlobalFilters=GlobalFilters&Name=Name&RejectedPatches=RejectedPatches",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15276e6a-b4d5-4d44-b0c8-f199c503577e"
            }
          ]
        }
      ]
    }
  ]
}