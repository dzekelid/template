---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Delete a category template
  description: Deletes a category template. The ID of the category, the plenty ID
    of the client (store) and the language must be specified.
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