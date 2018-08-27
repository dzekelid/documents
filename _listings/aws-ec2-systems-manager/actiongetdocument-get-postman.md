{
  "info": {
    "name": "Amazon EC2 Systems Manager API Get Document",
    "_postman_id": "2d0d80c6-2113-4d03-b026-1d039fe05225",
    "description": "Gets the contents of the specified SSM document.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "32257e92-0e5e-4a10-a43f-c226e1631437",
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
              "id": "79ad801f-650d-4509-8c6b-c59c70a8fb8d"
            }
          ]
        }
      ]
    },
    {
      "name": "Cancel",
      "item": [
        {
          "id": "1a3a205c-e70a-480c-afe2-5cd64449af1a",
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
              "id": "da4bfbb4-5999-4972-b901-10cef9b9871b"
            }
          ]
        }
      ]
    },
    {
      "name": "Activation",
      "item": [
        {
          "id": "616ce209-c161-4956-b41c-0c4600ef7ac8",
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
              "id": "fb539f0b-5d75-4053-8c86-aef242af647c"
            }
          ]
        },
        {
          "id": "82c66921-7b1a-4439-9a54-62d426115e2d",
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
              "id": "6c9f2671-3015-44f4-91be-cbfc3b5ba1a2"
            }
          ]
        }
      ]
    },
    {
      "name": "Association",
      "item": [
        {
          "id": "0bf4123d-fd2e-470a-ad21-fb1ca23ca9a9",
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
              "id": "5b6da5c7-e1d1-46a3-b332-5b634de49601"
            }
          ]
        },
        {
          "id": "358bfd56-961f-4d4e-94cd-03fab5bbfb22",
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
              "id": "710d0d4a-af39-4822-b3de-6b3564115531"
            }
          ]
        },
        {
          "id": "4974db48-82c5-4d99-9823-effa5e95f93c",
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
              "id": "8c7e39c3-b073-482f-8588-0841cd1cb9b3"
            }
          ]
        },
        {
          "id": "4aa16726-0b15-4361-879b-491cedfa4a5c",
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
              "id": "61fc007a-323a-4633-9fdb-dd49e775ee15"
            }
          ]
        }
      ]
    },
    {
      "name": "Document",
      "item": [
        {
          "id": "23d55b09-dc25-4da9-8665-f636063a6bc2",
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
              "id": "7be07a63-8348-47ca-a667-604e63a2b9d4"
            }
          ]
        },
        {
          "id": "101c29ae-dacb-48ba-9bb6-9a416ace5b49",
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
              "id": "008897a1-1995-40f2-ba7f-fed096ac50c5"
            }
          ]
        },
        {
          "id": "ceb43ec7-ee2d-4e63-9750-3fb139c6fce9",
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
              "id": "fd767180-bb25-4311-8764-55a9862262a9"
            }
          ]
        },
        {
          "id": "1c7eacbf-4c0a-4ef8-b78a-6030d92f3cb3",
          "name": "describeDocumentPermission",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDocumentPermission?Name=Name&PermissionType=PermissionType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the permissions for an SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eae8fb98-aa52-4002-8377-a3ae72f4a16a"
            }
          ]
        },
        {
          "id": "466c2552-7d51-4f7f-b385-238c8c66dc9d",
          "name": "getDocument",
          "request": {
            "url": "http://example.com/api/?Action=GetDocument?DocumentVersion=DocumentVersion&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the contents of the specified SSM document."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd8deca1-79bf-4cba-86ab-86b5c07e9870"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "b5a53159-37ca-4fba-8456-665328aa587c",
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
              "id": "3fab3b04-82e5-496a-acab-ae8c84e5dce5"
            }
          ]
        },
        {
          "id": "dcdc7a6d-6490-4d05-9e7e-1bae36e7ea13",
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
              "id": "5c807e41-4906-4376-9cac-43811f968a8a"
            }
          ]
        },
        {
          "id": "13f2371d-c513-450b-a6ec-fcad190a36a4",
          "name": "describeMaintenanceWindowExecutions",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutions?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the executions of a Maintenance Window (meaning, information about when the\n   Maintenance Window was scheduled to be active and information about tasks registered and run with\n   the Maintenance Window)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6cf701d-3daf-4ab1-b3bf-6cbe6c86e4b7"
            }
          ]
        },
        {
          "id": "fa2f0679-ad2a-4d82-b5f4-e70c55c96b75",
          "name": "describeMaintenanceWindowExecutionTaskInvocations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTaskInvocations?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&TaskId=TaskId&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the individual task executions (one per target) for a particular task executed\n   as part of a Maintenance Window execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c684a568-f8e8-4ec6-95a2-eaff90f8e851"
            }
          ]
        },
        {
          "id": "ee99bd87-0422-4bb9-86fa-ccb873915ae1",
          "name": "describeMaintenanceWindowExecutionTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowExecutionTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowExecutionId=WindowExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a given Maintenance Window execution, lists the tasks that were executed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22534aac-801d-4914-81e1-4e826bc99f32"
            }
          ]
        },
        {
          "id": "ee160bef-6253-4fb4-87aa-db5a0fc3df58",
          "name": "describeMaintenanceWindows",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindows?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the Maintenance Windows in an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c52dc47c-d0aa-4e2a-a20e-28bfcfe7d58a"
            }
          ]
        },
        {
          "id": "7c3ea1df-4169-4a4c-b7ad-b869c1d4d33a",
          "name": "describeMaintenanceWindowTargets",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTargets?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the targets registered with the Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4a1e6a2-46b7-4077-b092-8d50f7d5c60c"
            }
          ]
        },
        {
          "id": "de62332f-d7c7-472d-87eb-29056a348814",
          "name": "describeMaintenanceWindowTasks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceWindowTasks?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&WindowId=WindowId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the tasks in a Maintenance Window."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5680fa41-6077-474c-987b-7054ad16cf8c"
            }
          ]
        }
      ]
    },
    {
      "name": "Baseline",
      "item": [
        {
          "id": "a54d1a76-540c-4a32-af5b-e790dbd6cd6a",
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
              "id": "1fdb2526-a970-42f5-99e8-bd3945254bfb"
            }
          ]
        },
        {
          "id": "8a806d3a-4b52-45d4-9ad2-c7074656927c",
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
              "id": "75cbe238-1499-47eb-aacc-c5dda6fe7ae1"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameter",
      "item": [
        {
          "id": "09d92121-95a6-4b19-b430-5fef2fe9b7fc",
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
              "id": "81a9c573-307a-4848-b309-e225e0761e5d"
            }
          ]
        }
      ]
    },
    {
      "name": "Deregister",
      "item": [
        {
          "id": "6041b690-3947-4240-a01e-c5f71e542875",
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
              "id": "6b66124f-7808-44a5-b37e-ab8c3b05ec64"
            }
          ]
        },
        {
          "id": "8ebba1d6-0ad4-4465-ba17-892192aab721",
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
              "id": "f7577246-f2aa-4956-8557-326a44c02f4d"
            }
          ]
        },
        {
          "id": "5205f8c4-5009-4b00-9057-af1daa43e8ae",
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
              "id": "d7fc0112-2b34-4c66-8045-d055b86ddc0d"
            }
          ]
        },
        {
          "id": "c6f43a1a-3dcb-447e-8fda-79129b81d1cd",
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
              "id": "97245a7c-5855-4eab-b070-79c9bb97fffe"
            }
          ]
        }
      ]
    },
    {
      "name": "Activations",
      "item": [
        {
          "id": "51567437-8ee9-4f3c-8500-e70dd0842d09",
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
              "id": "710c520c-f194-4af9-8f2f-776c8e056869"
            }
          ]
        }
      ]
    },
    {
      "name": "Automation",
      "item": [
        {
          "id": "ba227efe-0fb5-4707-a30d-ea4fea03897e",
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
              "id": "83b1957e-a6ba-4c3b-8b22-edfecbe8ab04"
            }
          ]
        },
        {
          "id": "385fb4ca-d0d2-4bcc-953f-54b860aed3b5",
          "name": "getAutomationExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetAutomationExecution?AutomationExecutionId=AutomationExecutionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get detailed information about a particular Automation execution."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e948173f-e3e9-4e95-addf-8d7f03b2f9cc"
            }
          ]
        }
      ]
    },
    {
      "name": "Available",
      "item": [
        {
          "id": "a66d767c-cb92-476d-a30b-d3c89ff84894",
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
              "id": "76a0464b-278a-4c64-ad69-cdaa4816b311"
            }
          ]
        }
      ]
    },
    {
      "name": "Effective",
      "item": [
        {
          "id": "b2ea63c3-e239-4ae6-8c7e-24acefd37e20",
          "name": "describeEffectiveInstanceAssociations",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectiveInstanceAssociations?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "All associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "18e9d64a-7a91-4881-b24e-9491d2b7a3da"
            }
          ]
        },
        {
          "id": "3c36847a-6ea7-4564-9d0a-c9fdf415b4fd",
          "name": "describeEffectivePatchesForPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEffectivePatchesForPatchBaseline?BaselineId=BaselineId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current effective patches (the patch and the approval state) for the specified patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1aa0a04-583f-4c51-8353-770ef508a1a6"
            }
          ]
        }
      ]
    },
    {
      "name": "Instance",
      "item": [
        {
          "id": "a2af65b5-f972-4e24-9fcb-436cf30d9377",
          "name": "describeInstanceAssociationsStatus",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceAssociationsStatus?InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The status of the associations for the instance(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cddf4584-3ac5-4993-bad6-f57eccf49c6f"
            }
          ]
        },
        {
          "id": "3865c886-eb2a-42a0-b892-2bd1101d43d5",
          "name": "describeInstanceInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstanceInformation?Filters=Filters&InstanceInformationFilterList=InstanceInformationFilterList&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes one or more of your instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d88dc76-eba1-4b62-b796-2b974ce7f607"
            }
          ]
        },
        {
          "id": "8475270c-e8cc-495f-8d59-5afee5f6e636",
          "name": "describeInstancePatches",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatches?Filters=Filters&InstanceId=InstanceId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves information about the patches on the specified instance and their state relative to the patch baseline being used for the instance."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16a038ba-ac1c-4cbb-aa78-35ee51370ea8"
            }
          ]
        },
        {
          "id": "78e6fb17-fd36-4f76-83af-d0cfb3b3cce6",
          "name": "describeInstancePatchStates",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStates?InstanceIds=InstanceIds&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state of one or more instances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ed14444-0ceb-4b61-a07c-a190b7ef2897"
            }
          ]
        },
        {
          "id": "27452719-25c2-4ea9-ae4e-e58a2be21c26",
          "name": "describeInstancePatchStatesForPatchGroup",
          "request": {
            "url": "http://example.com/api/?Action=DescribeInstancePatchStatesForPatchGroup?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken&PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the high-level patch state for the instances in the specified patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8ac9291-e2b1-4cfb-858d-582fb746d3f6"
            }
          ]
        }
      ]
    },
    {
      "name": "Parameters",
      "item": [
        {
          "id": "a3070c26-8189-47d3-938c-c515b0553857",
          "name": "describeParameters",
          "request": {
            "url": "http://example.com/api/?Action=DescribeParameters?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get information about a parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34d02332-500c-4970-8304-7c26e19a9e7d"
            }
          ]
        }
      ]
    },
    {
      "name": "Baselines",
      "item": [
        {
          "id": "d1d324e1-b414-48e0-ae7b-154eac5ebadc",
          "name": "describePatchBaselines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchBaselines?Filters=Filters&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the patch baselines in your AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48e0475a-9f29-4038-a722-98709e63f463"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "967b5c07-6fff-4c94-b60d-62a9a66e8282",
          "name": "describePatchGroups",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroups?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all patch groups that have been registered with patch baselines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b54b2e96-0c60-4fe3-baa0-5e9b4311f7de"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "930a40bc-924b-4ab3-883d-818cb028a056",
          "name": "describePatchGroupState",
          "request": {
            "url": "http://example.com/api/?Action=DescribePatchGroupState?PatchGroup=PatchGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns high-level aggregated patch compliance state for a patch group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8acf75d4-6a21-433e-81ac-6b99c7688fa4"
            }
          ]
        }
      ]
    },
    {
      "name": "Command",
      "item": [
        {
          "id": "36e63356-b8dd-43ed-ab9c-47e2041f71d5",
          "name": "getCommandInvocation",
          "request": {
            "url": "http://example.com/api/?Action=GetCommandInvocation?CommandId=CommandId&InstanceId=InstanceId&PluginName=PluginName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns detailed information about command execution for an invocation or plugin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fd20ab5-d7bf-48ab-87d5-84561c689fa4"
            }
          ]
        }
      ]
    },
    {
      "name": "Default",
      "item": [
        {
          "id": "8a70653d-6790-448c-98b0-f60b47dca081",
          "name": "getDefaultPatchBaseline",
          "request": {
            "url": "http://example.com/api/?Action=GetDefaultPatchBaseline?BaselineId=BaselineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the default patch baseline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1953c6e-d9db-4556-9b89-73309786ab89"
            }
          ]
        }
      ]
    },
    {
      "name": "Deployable",
      "item": [
        {
          "id": "6858c098-e5b8-4420-a39a-3a52ff25f077",
          "name": "getDeployablePatchSnapshotForInstance",
          "request": {
            "url": "http://example.com/api/?Action=GetDeployablePatchSnapshotForInstance?InstanceId=InstanceId&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the current snapshot for the patch baseline the instance uses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c12b001-ad0c-42b6-ad86-5c7f6e5892be"
            }
          ]
        }
      ]
    }
  ]
}