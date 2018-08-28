swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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
    delete:
      summary: Remove template
      description: "Deletes a template. This results in different actions depending
        on the \ntype of template:\n\n- If the template is a content template, it
        is deleted.\n- If the template is a modified space-level blueprint template,
        it reverts \nto the template inherited from the global-level blueprint template.\n-
        If the template is a modified global-level blueprint template, it reverts
        \nto the default global-level blueprint template.\n\n Note, unmodified blueprint
        templates cannot be deleted."
      operationId: com.atlassian.confluence.plugins.restapi.resources.TemplateResource.removeTemplate_delete
      x-api-path-slug: templatecontenttemplateid-delete
      parameters:
      - in: path
        name: contentTemplateId
        description: The ID of the template to be deleted
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Template