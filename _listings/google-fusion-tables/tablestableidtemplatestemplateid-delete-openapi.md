---
swagger: "2.0"
x-collection-name: Google Fusion Tables
x-complete: 0
info:
  title: Google Fusion Tables API Delete Template
  description: Deletes a template
  contact:
    name: Google
    url: https://google.com
  version: v2
host: www.googleapis.com
basePath: /fusiontables/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tables/{tableId}/templates:
    get:
      summary: Get Templates
      description: Retrieves a list of templates.
      operationId: fusiontables.template.list
      x-api-path-slug: tablestableidtemplates-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of templates to return
      - in: query
        name: pageToken
        description: Continuation token specifying which results page to return
      - in: path
        name: tableId
        description: Identifier for the table whose templates are being requested
      responses:
        200:
          description: OK
      tags:
      - Template
    post:
      summary: Create Template
      description: Creates a new template for the table.
      operationId: fusiontables.template.insert
      x-api-path-slug: tablestableidtemplates-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: tableId
        description: Table for which a new template is being created
      responses:
        200:
          description: OK
      tags:
      - Template
  /tables/{tableId}/templates/{templateId}:
    delete:
      summary: Delete Template
      description: Deletes a template
      operationId: fusiontables.template.delete
      x-api-path-slug: tablestableidtemplatestemplateid-delete
      parameters:
      - in: path
        name: tableId
        description: Table from which the template is being deleted
      - in: path
        name: templateId
        description: Identifier for the template which is being deleted
      responses:
        200:
          description: OK
      tags:
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