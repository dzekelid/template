---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Uploads an operational template.
  description: Uploads an operational template..
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /rest/v1
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