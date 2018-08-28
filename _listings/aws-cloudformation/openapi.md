swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 1
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=EstimateTemplateCost:
    get:
      summary: Estimate Template Cost
      description: Returns the estimated monthly cost of a template.
      operationId: estimateTemplateCost
      x-api-path-slug: actionestimatetemplatecost-get
      parameters:
      - in: query
        name: Parameters.member.N
        description: A list of Parameter structures that specify input parameters
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      responses:
        200:
          description: OK
      tags:
      - Template Cost
  /?Action=GetTemplate:
    get:
      summary: Get Template
      description: Returns the template body for a specified stack.
      operationId: getTemplate
      x-api-path-slug: actiongettemplate-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of a change set for which
          AWS CloudFormation returns the associated template
        type: string
      - in: query
        name: StackName
        description: 'The name or the unique stack ID that is associated with the
          stack, which are not always interchangeable:'
        type: string
      - in: query
        name: TemplateStage
        description: For templates that include transforms, the stage of the template
          that AWS CloudFormation returns
        type: string
      responses:
        200:
          description: OK
      tags:
      - Templates
  /?Action=GetTemplateSummary:
    get:
      summary: Get Template Summary
      description: Returns information about a new or existing template.
      operationId: getTemplateSummary
      x-api-path-slug: actiongettemplatesummary-get
      parameters:
      - in: query
        name: StackName
        description: The name or the stack ID that is associated with the stack, which
          are not always interchangeable
        type: string
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      responses:
        200:
          description: OK
      tags:
      - Templates
  /?Action=ValidateTemplate:
    get:
      summary: Validate Template
      description: Validates a specified template.
      operationId: validateTemplate
      x-api-path-slug: actionvalidatetemplate-get
      parameters:
      - in: query
        name: TemplateBody
        description: Structure containing the template body with a minimum length
          of 1 byte and a maximum length of 51,200 bytes
        type: string
      - in: query
        name: TemplateURL
        description: Location of file containing the template body
        type: string
      responses:
        200:
          description: OK
      tags:
      - Templates