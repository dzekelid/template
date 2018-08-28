swagger: "2.0"
x-collection-name: EhrScape
x-complete: 1
info:
  title: EhrScape Terminology APIs
  description: validates-and-resolves-terminology-codes
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /terminology-adapter/rest
paths:
  /template:
    get:
      summary: Gets all template ids.
      description: Gets all template ids..
      operationId: getAllTemplates
      x-api-path-slug: template-get
      responses:
        200:
          description: OK
      tags:
      - Template
    post:
      summary: Uploads an operational template.
      description: Uploads an operational template..
      operationId: saveTemplate
      x-api-path-slug: template-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Template
  /template/{templateId}:
    delete:
      summary: Deletes an existing OpenEHR template.
      description: Deletes an existing openehr template..
      operationId: deleteTemplate
      x-api-path-slug: templatetemplateid-delete
      parameters:
      - in: path
        name: templateId
        description: The ID of the template to delete
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
    get:
      summary: Loads an OpenEhr web template.
      description: Loads an openehr web template..
      operationId: getTemplate
      x-api-path-slug: templatetemplateid-get
      parameters:
      - in: query
        name: defaultLanguage
        description: The default language to generate the returned web template with
      - in: query
        name: languages
        description: Other languages to include in the returned web template, separated
          by a comma
      - in: path
        name: templateId
        description: The ID of the template to load
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
  /template/{templateId}/example:
    get:
      summary: Returns an example of data values for a web template.
      description: Returns an example of data values for a web template..
      operationId: getTemplateExample
      x-api-path-slug: templatetemplateidexample-get
      parameters:
      - in: query
        name: defaultLanguage
        description: The default language to generate the web template with
      - in: query
        name: exampleFilter
        description: The type of example to produce - intended for input (sent to
          the server), output (received back from the server) etc
      - in: query
        name: format
        description: The format of JSON representation of the example composition
          to return
      - in: query
        name: languages
        description: Other languages to include in the web template, separated by
          a comma
      - in: path
        name: templateId
        description: The ID of the template to load
      responses:
        200:
          description: OK
      tags:
      - Template
      - TemplateId
      - Example