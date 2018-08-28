---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Update the properties of a template, but not its content.
  version: 1.0.0
  description: Update the properties of a template, but not its content..
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
  /api/documentgeneration/lettertemplate/properties/{id}:
    post:
      summary: Update the properties of a template, but not its content.
      description: Update the properties of a template, but not its content..
      operationId: DocumentGeneration_UpdateLetterTemplatePropertiesByidBytemplatePropertiesSaveDataContract
      x-api-path-slug: apidocumentgenerationlettertemplatepropertiesid-post
      parameters:
      - in: path
        name: id
        description: Document Id for the template
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: templatePropertiesSaveDataContract
        description: The letter template property changes
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Properties
      - Of
      - Template
      - ""
      - But
      - Not
      - Its
      - Content
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