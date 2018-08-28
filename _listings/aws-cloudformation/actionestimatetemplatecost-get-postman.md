{
  "info": {
    "name": "AWS CloudFormation API Estimate Template Cost",
    "_postman_id": "ae65448a-2d8b-4d3c-aa0e-a3d80a7b2958",
    "description": "Returns the estimated monthly cost of a template.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Stacks",
      "item": [
        {
          "id": "c3e8239e-d26d-4808-a08e-7db907093b05",
          "name": "cancelUpdateStack",
          "request": {
            "url": "http://example.com/api/?Action=CancelUpdateStack?StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an update on the specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8fb8af9c-e306-44a0-a6fe-e689df1d0d59"
            }
          ]
        },
        {
          "id": "a2db5c37-698a-4690-9096-55a08b71fa7f",
          "name": "createStack",
          "request": {
            "url": "http://example.com/api/?Action=CreateStack?Capabilities.member.N=Capabilities.member.N&DisableRollback=DisableRollback&NotificationARNs.member.N=NotificationARNs.member.N&OnFailure=OnFailure&Parameters.member.N=Parameters.member.N&ResourceTypes.member.N=ResourceTypes.member.N&RoleARN=RoleARN&StackName=StackName&StackPolicyBody=StackPolicyBody&StackPolicyURL=StackPolicyURL&Tags.member.N=Tags.member.N&TemplateBody=TemplateBody&TemplateURL=TemplateURL&TimeoutInMinutes=TimeoutInMinutes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a stack as specified in the template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05cc5fc9-c469-4267-9393-bf3a6f7fd78b"
            }
          ]
        },
        {
          "id": "451ed88e-2d3c-45fe-acc6-0986ffa74109",
          "name": "deleteStack",
          "request": {
            "url": "http://example.com/api/?Action=DeleteStack?RetainResources.member.N=RetainResources.member.N&RoleARN=RoleARN&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07f9cc8c-554d-4fd9-b973-725ca854ec89"
            }
          ]
        },
        {
          "id": "8b46b6fd-8d83-4e48-802e-648bda4294a5",
          "name": "describeStacks",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStacks?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the description for the specified stack; if no stack name was specified, then it returns the description for all the stacks created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b96e2f1-9b06-42e9-b29b-7b40a4e21943"
            }
          ]
        }
      ]
    },
    {
      "name": "Rollback",
      "item": [
        {
          "id": "74c3c945-2b73-4553-8e30-004bca3100fb",
          "name": "continueUpdateRollback",
          "request": {
            "url": "http://example.com/api/?Action=ContinueUpdateRollback?ResourcesToSkip.member.N=ResourcesToSkip.member.N&RoleARN=RoleARN&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "For a specified stack that is in the UPDATE_ROLLBACK_FAILED state, continues rolling it back\n         to the UPDATE_ROLLBACK_COMPLETE state."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59a813af-87ec-4c59-9105-2fe58aa5f115"
            }
          ]
        }
      ]
    },
    {
      "name": "Change Sets",
      "item": [
        {
          "id": "99ce6696-6f2d-411a-b324-296ddd4ace74",
          "name": "createChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=CreateChangeSet?Capabilities.member.N=Capabilities.member.N&ChangeSetName=ChangeSetName&ChangeSetType=ChangeSetType&ClientToken=ClientToken&Description=Description&NotificationARNs.member.N=NotificationARNs.member.N&Parameters.member.N=Parameters.member.N&ResourceTypes.member.N=ResourceTypes.member.N&RoleARN=RoleARN&StackName=StackName&Tags.member.N=Tags.member.N&TemplateBody=TemplateBody&TemplateURL=TemplateURL&UsePreviousTemplate=UsePreviousTemplate",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a list of changes for a stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea4687ad-c70c-4bce-8203-6c8ba3dda848"
            }
          ]
        },
        {
          "id": "e262fdaa-28a7-401a-86f1-a78ae9dadd23",
          "name": "deleteChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=DeleteChangeSet?ChangeSetName=ChangeSetName&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified change set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7459efc-a36e-4639-b2de-a65cc9bab509"
            }
          ]
        },
        {
          "id": "30a3b77a-6d10-40c3-b71d-899a0ce6ac78",
          "name": "describeChangeSet",
          "request": {
            "url": "http://example.com/api/?Action=DescribeChangeSet?ChangeSetName=ChangeSetName&NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the inputs for the change set and a list of changes that AWS CloudFormation will make if you execute the change set."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd9b3f5b-a136-48ab-89bc-9ca19e294c4c"
            }
          ]
        }
      ]
    },
    {
      "name": "Account Limits",
      "item": [
        {
          "id": "210e218c-cecb-4d09-94cf-4943c4778edf",
          "name": "describeAccountLimits",
          "request": {
            "url": "http://example.com/api/?Action=DescribeAccountLimits?NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves your account's AWS CloudFormation limits, such as the maximum number of stacks that you can create in your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f243894a-cac5-4a53-8164-fe81c8db84c9"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Events",
      "item": [
        {
          "id": "f271b879-eed7-46b6-b3ad-466f8aac3aeb",
          "name": "describeStackEvents",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackEvents?NextToken=NextToken&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all stack related events for a specified stack in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90aed105-38cd-4622-9648-74aa651c2ab6"
            }
          ]
        }
      ]
    },
    {
      "name": "Stack Resources",
      "item": [
        {
          "id": "4195a7f5-831b-448c-9083-50717ecdfea7",
          "name": "describeStackResource",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackResource?LogicalResourceId=LogicalResourceId&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the specified resource in the specified stack."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ecd8607-0327-4380-98bf-514f090199a5"
            }
          ]
        },
        {
          "id": "f82587b8-aaca-4bc4-83c7-de4abaeec003",
          "name": "describeStackResources",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStackResources?LogicalResourceId=LogicalResourceId&PhysicalResourceId=PhysicalResourceId&StackName=StackName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns AWS resource descriptions for running and deleted stacks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4764f7d3-8339-4a4b-b8b8-b4caea58d75d"
            }
          ]
        }
      ]
    },
    {
      "name": "Template Cost",
      "item": [
        {
          "id": "37c6bb4c-7d5a-4ed2-8b08-b39a5330b1cf",
          "name": "estimateTemplateCost",
          "request": {
            "url": "http://example.com/api/?Action=EstimateTemplateCost?Parameters.member.N=Parameters.member.N&TemplateBody=TemplateBody&TemplateURL=TemplateURL",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the estimated monthly cost of a template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "285635b2-0abe-4745-a88a-f65a110da1f1"
            }
          ]
        }
      ]
    }
  ]
}