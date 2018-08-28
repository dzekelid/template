---
swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 0
info:
  title: AWS Elastic Beanstalk API Create Configuration Template
  version: 1.0.0
  description: Creates a configuration template.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateConfigurationTemplate:
    get:
      summary: Create Configuration Template
      description: Creates a configuration template.
      operationId: createConfigurationTemplate
      x-api-path-slug: actioncreateconfigurationtemplate-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to associate with this configuration
          template
        type: string
      - in: query
        name: Description
        description: Describes this configuration
        type: string
      - in: query
        name: EnvironmentId
        description: The ID of the environment used with this configuration template
        type: string
      - in: query
        name: OptionSettings.member.N
        description: If specified, AWS Elastic Beanstalk sets the specified configuration
          option to the      requested value
        type: string
      - in: query
        name: SolutionStackName
        description: The name of the solution stack used by this configuration
        type: string
      - in: query
        name: SourceConfiguration
        description: If specified, AWS Elastic Beanstalk uses the configuration values
          from the specified      configuration template to create a new configuration
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Templates
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---