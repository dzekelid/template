---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: "Dezrez Does a simple merge of the selected envelopeTemplatePack using the
    data supplied\r\nwill only use certain merge functions, and the correspondence
    can only contain one envelope and the envelope can only contain one document."
  version: 1.0.0
  description: "Does a simple merge of the selected envelopetemplatepack using the
    data supplied\r\nwill only use certain merge functions, and the correspondence
    can only contain one envelope and the envelope can only contain one document.."
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
  /api/documentgeneration/updateheadertemplate/{id}/{brandId}:
    post:
      summary: Updates a header letter template
      description: Updates a header letter template.
      operationId: DocumentGeneration_UpdateHeaderTemplateByidBybrandIdByletterTemplate
      x-api-path-slug: apidocumentgenerationupdateheadertemplateidbrandid-post
      parameters:
      - in: path
        name: brandId
        description: Brand Id for this header
      - in: path
        name: id
        description: Document Id
      - in: body
        name: letterTemplate
        description: The header template
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
      - Header
      - Letter
      - Template
  /api/documentgeneration/saveenvelopetemplatepack:
    post:
      summary: Saves or updates envelope template correspondence for a an agency
      description: Saves or updates envelope template correspondence for a an agency.
      operationId: DocumentGeneration_SaveEnvelopeTemplatePackByenvelopeTemplatePack
      x-api-path-slug: apidocumentgenerationsaveenvelopetemplatepack-post
      parameters:
      - in: body
        name: envelopeTemplatePack
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Saves
      - Updates
      - Envelope
      - Template
      - Correspondencea
      - Agency
  /api/documentgeneration/envelopetemplate/{id}:
    get:
      summary: Returns a envelope template
      description: Returns a envelope template.
      operationId: DocumentGeneration_GetEnvelopeTemplateByid
      x-api-path-slug: apidocumentgenerationenvelopetemplateid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Envelope
      - Template
  /api/documentgeneration/envelopetemplatepack/{id}:
    get:
      summary: Returns a envelope template pack
      description: Returns a envelope template pack.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackByid
      x-api-path-slug: apidocumentgenerationenvelopetemplatepackid-get
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Envelope
      - Template
      - Pack
  /api/documentgeneration/envelopetemplatepacks:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePacks
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacks-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacktypes:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackTypesByinUseOnly
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacktypes-get
      parameters:
      - in: query
        name: inUseOnly
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/deleteenvelopetemplatepack/{id}:
    delete:
      summary: Deletes a Envelope Template Correspondence
      description: Deletes a envelope template correspondence.
      operationId: DocumentGeneration_DeleteEnvelopeTemplatePackByid
      x-api-path-slug: apidocumentgenerationdeleteenvelopetemplatepackid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Envelope
      - Template
      - Correspondence
  /api/documentgeneration/deleteenvelopetemplate/{id}:
    delete:
      summary: Deletes a Envelope Template
      description: Deletes a envelope template.
      operationId: DocumentGeneration_DeleteEnvelopeTemplateByid
      x-api-path-slug: apidocumentgenerationdeleteenvelopetemplateid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Envelope
      - Template
  /api/documentgeneration/deletelettertemplate/{id}/{useageLimit}:
    delete:
      summary: Deletes a Letter Template
      description: Deletes a letter template.
      operationId: DocumentGeneration_DeleteLetterTemplateByidByuseageLimit
      x-api-path-slug: apidocumentgenerationdeletelettertemplateiduseagelimit-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: useageLimit
      responses:
        200:
          description: OK
      tags:
      - S
      - Letter
      - Template
  /api/documentgeneration/templateusagecount:
    get:
      summary: Get the usage count for a template in envelopes
      description: Get the usage count for a template in envelopes.
      operationId: DocumentGeneration_getDocumentSubTypesBytemplateId
      x-api-path-slug: apidocumentgenerationtemplateusagecount-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: templateId
      responses:
        200:
          description: OK
      tags:
      - Usage
      - Counta
      - Template
      - In
      - Envelopes
  /api/branding/uploademailtemplate:
    post:
      summary: Upload the data to create a Email Document Template for a Brand.
      description: Upload the data to create a email document template for a brand..
      operationId: Branding_UploadEmailTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploademailtemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - Email
      - Document
      - Templatea
      - Brand
  /api/branding/uploadsmstemplate:
    post:
      summary: Upload the data to create a SMS Document Template for a Brand.
      description: Upload the data to create a sms document template for a brand..
      operationId: Branding_UploadSMSTemplateBybrandTemplateSaveDataContract
      x-api-path-slug: apibrandinguploadsmstemplate-post
      parameters:
      - in: body
        name: brandTemplateSaveDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Data
      - To
      - Create
      - SMS
      - Document
      - Templatea
      - Brand
  /api/documentgeneration/envelopetemplatepacksummary/{envelopeTemplatePackId}:
    get:
      summary: Gets a list of the packs for a particular packtype
      description: Gets a list of the packs for a particular packtype.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackSummaryByenvelopeTemplatePackId
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacksummaryenvelopetemplatepackid-get
      parameters:
      - in: path
        name: envelopeTemplatePackId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Packsa
      - Particular
      - Packtype
  /api/documentgeneration/lettertemplate/{letterTemplateId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetLetterTemplateByletterTemplateId
      x-api-path-slug: apidocumentgenerationlettertemplatelettertemplateid-get
      parameters:
      - in: path
        name: letterTemplateId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/stationary/html/{brandId}:
    get:
      summary: "Does a simple merge of the selected envelopeTemplatePack using the
        data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document."
      description: "Does a simple merge of the selected envelopetemplatepack using
        the data supplied\r\nwill only use certain merge functions, and the correspondence
        can only contain one envelope and the envelope can only contain one document.."
      operationId: Stationary_HtmlStationaryBybrandId
      x-api-path-slug: apistationaryhtmlbrandid-get
      parameters:
      - in: path
        name: brandId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Does
      - Simple
      - Merge
      - Of
      - Selected
      - EnvelopeTemplatePack
      - Using
      - Data
      - "Supplied\r\nWill"
      - Only
      - Use
      - Certain
      - Merge
      - Functions
      - ""
      - Correspondence
      - Can
      - Only
      - Contain
      - Envelope
      - Envelope
      - Can
      - Only
      - Contain
      - Document
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