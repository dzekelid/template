swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
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
  /?Action=DeleteConfigurationTemplate:
    get:
      summary: Delete Configuration Template
      description: Deletes the specified configuration template.
      operationId: deleteConfigurationTemplate
      x-api-path-slug: actiondeleteconfigurationtemplate-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application to delete the configuration template
          from
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Templates
  /?Action=UpdateConfigurationTemplate:
    get:
      summary: Update Configuration Template
      description: |-
        Updates the specified configuration template to have the specified properties or
              configuration option values.
      operationId: updateConfigurationTemplate
      x-api-path-slug: actionupdateconfigurationtemplate-get
      parameters:
      - in: query
        name: ApplicationName
        description: The name of the application associated with the configuration
          template to      update
        type: string
      - in: query
        name: Description
        description: A new description for the configuration
        type: string
      - in: query
        name: OptionSettings.member.N
        description: A list of configuration option settings to update with the new
          specified option      value
        type: string
      - in: query
        name: OptionsToRemove.member.N
        description: A list of configuration options to remove from the configuration
          set
        type: string
      - in: query
        name: TemplateName
        description: The name of the configuration template to update
        type: string
      responses:
        200:
          description: OK
      tags:
      - Configuration Templates