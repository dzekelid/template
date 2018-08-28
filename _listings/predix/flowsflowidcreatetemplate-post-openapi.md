---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Insights Post Flows Flowid Create Template
  description: Post flows flowid create template.
  termsOfService: urn:tos
  version: 1.0.0
host: insights-api.data-services.predix.io
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /flows/{flowId}/create-template:
    post:
      summary: Post Flows Flowid Create Template
      description: Post flows flowid create template.
      operationId: createTemplateFromDirectFlowUsingPOST
      x-api-path-slug: flowsflowidcreatetemplate-post
      parameters:
      - in: path
        name: flowId
        description: flowId
      responses:
        200:
          description: Successful response
      tags:
      - Flows
      - Flowid
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