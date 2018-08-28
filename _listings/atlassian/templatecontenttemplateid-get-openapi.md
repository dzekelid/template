---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Get content template
  description: "Returns a content template. This includes information about template,
    \nlike the name, the space or blueprint that the template is in, the body \nof
    the template, and more.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \n'Admin' permission for the space to view space templates and 'Confluence
    \nAdministrator' global permission to view global templates."
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /template:
    post:
      summary: Create content template
      description: "Creates a new content template. Note, blueprint templates cannot
        be created via the REST API.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Admin' permission for the space to create a space template
        or 'Confluence Administrator' \nglobal permission to create a global template."
      operationId: com.atlassian.confluence.plugins.restapi.resources.TemplateResource.createContentTemplate_post
      x-api-path-slug: template-post
      responses:
        200:
          description: OK
      tags:
      - Content
      - Template
    put:
      summary: Update content template
      description: "Updates a content template. Note, blueprint templates cannot be
        updated\nvia the REST API.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Admin' permission for the space to create a space template
        or 'Confluence Administrator' \nglobal permission to create a global template."
      operationId: com.atlassian.confluence.plugins.restapi.resources.TemplateResource.updateContentTemplate_put
      x-api-path-slug: template-put
      responses:
        200:
          description: OK
      tags:
      - Content
      - Template
  /template/{contentTemplateId}:
    get:
      summary: Get content template
      description: "Returns a content template. This includes information about template,
        \nlike the name, the space or blueprint that the template is in, the body
        \nof the template, and more.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Admin' permission for the space to view space templates and
        'Confluence \nAdministrator' global permission to view global templates."
      operationId: com.atlassian.confluence.plugins.restapi.resources.TemplateResource.getContentTemplate_get
      x-api-path-slug: templatecontenttemplateid-get
      parameters:
      - in: path
        name: contentTemplateId
        description: The ID of the content template to be returned
      responses:
        200:
          description: OK
      tags:
      - Content
      - Template
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