---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get Metadata Template
  description: Used to retrieve the schema for a given metadata template.
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