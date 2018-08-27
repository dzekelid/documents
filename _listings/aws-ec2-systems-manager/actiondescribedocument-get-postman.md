{
  "info": {
    "name": "Amazon EC2 Systems Manager API Describe Document",
    "_postman_id": "2290230b-c106-4590-95a6-98024ed898cd",
    "description": "Describes the specified SSM document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "57eb5379-22da-4224-97ff-9d94b08c436b",
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
              "id": "9815485a-aedc-49c1-90fa-13dbd5a827ab"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "b271fa83-7ada-4129-806a-169a4040ed3c",
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
              "id": "c7069877-3820-43a8-9ad3-5274744e053d"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "2339fa6c-033d-4e24-8a28-af2571b5e53f",
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
              "id": "acd9a73d-2a32-4cd4-8866-8a5ee2c91597"
            }
          ]
        },
        {
          "id": "862c8250-49dd-4caf-816c-02f8aa160060",
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
              "id": "b35220b1-33e8-40d5-a162-f5cde6726239"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "833fadf1-c1dc-4d28-b6c8-d8bc635cc994",
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
              "id": "9ed0d43d-17f1-4165-9780-d6b36a3e9705"
            }
          ]
        },
        {
          "id": "64d03c11-8561-4435-9136-0fbaaff7c7c7",
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
              "id": "c3aabce2-32fe-4581-bbd0-d047fb6dfc47"
            }
          ]
        },
        {
          "id": "14879fc0-1702-45dd-abde-db4cc6341118",
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
              "id": "474ed67e-00db-4660-9dfe-9e1cd12276d0"
            }
          ]
        },
        {
          "id": "070920d9-5c07-4c04-af82-3b3685a9c563",
          "name": "describeAssociation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAssociation?AssociationId=AssociationId&InstanceId=InstanceId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the associations for the specified SSM document or instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "578c99a5-468c-4536-bea4-1c904896d71d"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "25055a2f-7e44-4377-9eb5-5ecfec399c72",
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
              "id": "0965e8d6-60c1-48ef-8250-b35f6383916a"
            }
          ]
        },
        {
          "id": "b1e05fc9-2de4-44fc-805f-a78b53e21fc5",
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
              "id": "f8cf26ab-95cd-4b0f-8c10-531c1e751394"
            }
          ]
        },
        {
          "id": "d5d1c3dd-05b0-4c8d-bcd2-9fafb998c556",
          "name": "describeDocument",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2156c90-5d1d-487f-bdce-bf5a87bf2feb"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "9da10c86-34c8-44ab-b5c8-03806ad3d174",
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
              "id": "425433f1-5842-40d6-8cf7-5d00f12899c1"
            }
          ]
        },
        {
          "id": "edc6ca07-0038-4510-b7db-82f89f357b85",
          "name": "deleteMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeleteMaintenanceWindow?WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d93d4e4-fbde-459d-96b4-ef713027a18e"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "eb76f2b1-7368-4ef6-ba5f-a0b74484bbca",
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
              "id": "a45ede2f-0a78-4f93-a9b0-844ceeb0b950"
            }
          ]
        },
        {
          "id": "efb9e2e1-a26d-4bc2-9320-6674a0ecb584",
          "name": "deletePatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71b85c16-b656-42c7-a177-74d3710ffa65"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "355c254f-6cff-4d0d-940d-fb61f07ea002",
          "name": "deleteParameter",
          "request": {
            "url": "http://example.com/api/?Action=DeleteParameter?Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a parameter from the system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be2e7c27-9ec9-4557-a95d-b050840883f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "1051cd86-bfe4-49e0-88c9-fb5a251b539f",
          "name": "deregisterManagedInstance",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterManagedInstance?InstanceId=InstanceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the server or virtual machine from the list of registered servers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1658a13-b32e-41dd-85ce-c28419ccb03e"
            }
          ]
        },
        {
          "id": "da8a3433-e728-4e6e-9195-204256bc8bbc",
          "name": "deregisterPatchBaselineForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterPatchBaselineForPatchGroup?BaselineId=BaselineId&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a patch group from a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a827b4e0-1a84-4948-abeb-8e06512d89da"
            }
          ]
        },
        {
          "id": "2458a854-bf0a-4da6-b89f-1d78b4258dd3",
          "name": "deregisterTargetFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTargetFromMaintenanceWindow?WindowId=WindowId&WindowTargetId=WindowTargetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a target from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d667a70-43e6-4f92-a888-987f55a169a1"
            }
          ]
        },
        {
          "id": "d5c5548a-dd2d-4aa4-b1ab-9050d5bcf4e9",
          "name": "deregisterTaskFromMaintenanceWindow",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterTaskFromMaintenanceWindow?WindowId=WindowId&WindowTaskId=WindowTaskId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a task from a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "206f8de3-0a14-4014-97ce-cd1b35fbaa3a"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "a201cd02-a3ad-4299-8f84-ebf9501c725c",
          "name": "describeActivations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeActivations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Details about the activation, including: the date and time the activation was created,\n   the expiration date, the IAM role assigned to the instances in the activation, and the number of\n   instances activated by this registration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8b9ff38-4f4f-4bf9-b03c-7215467f7dfc"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "1086ac9f-4592-49e0-b441-5273bcc5d86a",
          "name": "describeAutomationExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAutomationExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides details about all active and terminated Automation executions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f86f577b-b396-4f67-ab1a-7bef0cad58c9"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "09943d23-ccee-41f9-a4d0-70df8d328a0b",
          "name": "describeAvailablePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAvailablePatches?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patches that could possibly be included in a patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba7e0809-84d7-4266-8d7d-6a5f1d6f870e"
            }
          ]
        }
      ]
    }
  ]
}