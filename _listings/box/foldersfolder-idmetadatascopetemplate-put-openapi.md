---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Update Metadata on Folder
  description: Used to update the template instance. Updates can be either add, replace,
    remove , or test. The template instance can only be updated if the template instance
    already exists. When editing metadata, only values that adhere to the metadata
    template schema will be accepted.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metadata_templates/{SCOPE}/{TEMPLATE}/schema:
    get:
      summary: Get Metadata Template
      description: Used to retrieve the schema for a given metadata template.
      operationId: getMetadataTemplate
      x-api-path-slug: metadata-templatesscopetemplateschema-get
      parameters:
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Metadata
      - Templates
      - Scope
      - Template
      - Schema
    put:
      summary: Update Metadata Template
      description: Used to update the schema of an existing template.
      operationId: updateMetadataTemplate
      x-api-path-slug: metadata-templatesscopetemplateschema-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Metadata
      - Templates
      - Scope
      - Template
      - Schema
  /files/{FILE_ID}/metadata/{SCOPE}/{TEMPLATE}:
    post:
      summary: Create Metadata on File
      description: Used to create the metadata template instance for a corresponding
        Box file. When creating metadata, only values that adhere to the metadata
        template schema will be accepted.
      operationId: createFileMetadata
      x-api-path-slug: filesfile-idmetadatascopetemplate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FILE_ID
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Metadata
      - Scope
      - Template
    get:
      summary: Get Metadata on File
      description: Used to retrieve the metadata template instance for a corresponding
        Box file.
      operationId: getFileMetadata
      x-api-path-slug: filesfile-idmetadatascopetemplate-get
      parameters:
      - in: path
        name: FILE_ID
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Metadata
      - Scope
      - Template
    put:
      summary: Update Metadata on File
      description: |-
        Used to update the template instance. The request body must follow the JSON-Patch specification, which is represented as a JSON array of operation objects (see examples for more details). Updates can be either add, replace, remove , test, move, or copy. The template instance can only be updated if the template instance already exists. When editing metadata, only values that adhere to the metadata template schema will be accepted.
        The update is applied atomically. If any errors occur during the application of the update operations, the metadata instance remains unchanged.
      operationId: updateFileMetadata
      x-api-path-slug: filesfile-idmetadatascopetemplate-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FILE_ID
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Metadata
      - Scope
      - Template
    delete:
      summary: Delete Metadata on File
      description: Used to delete the template instance. To delete custom key:value
        pairs within a template instance, you should refer to the updating metadata
        section.
      operationId: deleteFileMetadata
      x-api-path-slug: filesfile-idmetadatascopetemplate-delete
      parameters:
      - in: path
        name: FILE_ID
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Files
      - File
      - ""
      - Metadata
      - Scope
      - Template
  /folders/{FOLDER_ID}/metadata/{SCOPE}/{TEMPLATE}:
    post:
      summary: Create Metadata on Folder
      description: Used to create the metadata template instance for a corresponding
        Box folder. When creating metadata, only values that adhere to the metadata
        template schema will be accepted.
      operationId: createFolderMetadata
      x-api-path-slug: foldersfolder-idmetadatascopetemplate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FOLDER_ID
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Folders
      - Folder
      - ""
      - Metadata
      - Scope
      - Template
    get:
      summary: Get Metadata on Folder
      description: Used to retrieve the metadata template instance for a corresponding
        Box folder.
      operationId: getFolderMetadata
      x-api-path-slug: foldersfolder-idmetadatascopetemplate-get
      parameters:
      - in: path
        name: FOLDER_ID
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Folders
      - Folder
      - ""
      - Metadata
      - Scope
      - Template
    put:
      summary: Update Metadata on Folder
      description: Used to update the template instance. Updates can be either add,
        replace, remove , or test. The template instance can only be updated if the
        template instance already exists. When editing metadata, only values that
        adhere to the metadata template schema will be accepted.
      operationId: updateFolderMetadata
      x-api-path-slug: foldersfolder-idmetadatascopetemplate-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FOLDER_ID
      - in: path
        name: SCOPE
      - in: path
        name: TEMPLATE
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Folders
      - Folder
      - ""
      - Metadata
      - Scope
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