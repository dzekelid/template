---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Get option template
  description: Gets an option template by ID.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/categories/{id}/templates:
    delete:
      summary: Delete a category template
      description: Deletes a category template. The ID of the category, the plenty
        ID of the client (store) and the language must be specified.
      operationId: deleteRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-delete
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
    get:
      summary: Get a category template
      description: Gets a category template. The ID of the category, the plenty ID
        of the client (store) and the language must be specified.
      operationId: getRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-get
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: lang
        description: The language of the template
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
    put:
      summary: Update a category template
      description: Updates a category template. The ID of the category, the plenty
        ID of the client (store) and the language must be specified.
      operationId: putRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-put
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
  /rest/listings/layout_templates:
    post:
      summary: Create new layout template
      description: Creates a new layout template.
      operationId: postRestListingsLayoutTemplates
      x-api-path-slug: restlistingslayout-templates-post
      parameters:
      - in: body
        name: /rest/listings/layout_templates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - New
      - Layout
      - Template
  /rest/listings/layout_templates/{id}:
    delete:
      summary: Delete a layout template
      description: Deletes a layout template by ID.
      operationId: deleteRestListingsLayoutTemplates
      x-api-path-slug: restlistingslayout-templatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Layout
      - Template
    get:
      summary: Get a layout template
      description: Gets a layout template by providing its ID.
      operationId: getRestListingsLayoutTemplates
      x-api-path-slug: restlistingslayout-templatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Layout
      - Template
  /rest/listings/option_templates:
    post:
      summary: Create option template
      description: Creates an option template.
      operationId: postRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templates-post
      parameters:
      - in: body
        name: /rest/listings/option_templates
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
  /rest/listings/option_templates/{id}:
    delete:
      summary: Delete option template
      description: Deletes an option template by ID.
      operationId: deleteRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templatesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Option
      - Template
    get:
      summary: Get option template
      description: Gets an option template by ID.
      operationId: getRestListingsOptionTemplates
      x-api-path-slug: restlistingsoption-templatesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Option
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