---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Rename a letter template and change the description
  version: 1.0.0
  description: Rename a letter template and change the description.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/createlettertemplate:
    post:
      summary: Uploads a new letter template
      description: Uploads a new letter template.
      operationId: DocumentGeneration_CreateLetterTemplateByletterTemplate
      x-api-path-slug: apidocumentgenerationcreatelettertemplate-post
      parameters:
      - in: body
        name: letterTemplate
        description: The letter template
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - New
      - Letter
      - Template
  /api/documentgeneration/createheadertemplate/{brandId}:
    post:
      summary: Uploads a new header template
      description: Uploads a new header template.
      operationId: DocumentGeneration_CreateHeaderTemplateBybrandIdByletterTemplate
      x-api-path-slug: apidocumentgenerationcreateheadertemplatebrandid-post
      parameters:
      - in: path
        name: brandId
        description: Brand Id for this header
      - in: body
        name: letterTemplate
        description: The letter template
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - New
      - Header
      - Template
  /api/documentgeneration/updatelettertemplate/{id}:
    post:
      summary: Updates a merge letter template
      description: Updates a merge letter template.
      operationId: DocumentGeneration_UpdateLetterTemplateByidByletterTemplate
      x-api-path-slug: apidocumentgenerationupdatelettertemplateid-post
      parameters:
      - in: path
        name: id
        description: Document Id for the template
      - in: body
        name: letterTemplate
        description: The letter template
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Merge
      - Letter
      - Template
  /api/documentgeneration/renamelettertemplate/{id}:
    post:
      summary: Rename a letter template and change the description
      description: Rename a letter template and change the description.
      operationId: DocumentGeneration_UpdateLetterTemplateByidByrenameDataContract
      x-api-path-slug: apidocumentgenerationrenamelettertemplateid-post
      parameters:
      - in: path
        name: id
        description: Document Id for the template
      - in: body
        name: renameDataContract
        description: The letter template
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Rename
      - Letter
      - Template
      - Change
      - Description
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