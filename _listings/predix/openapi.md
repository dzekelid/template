swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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