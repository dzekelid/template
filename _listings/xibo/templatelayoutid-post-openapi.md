---
swagger: "2.0"
x-collection-name: Xibo
x-complete: 0
info:
  title: Xibo API Add a template from a Layout
  description: Use the provided layout as a base for a new template
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /template:
    get:
      summary: Template Search
      description: Search templates this user has access to
      operationId: templateSearch
      x-api-path-slug: template-get
      responses:
        200:
          description: OK
      tags:
      - Template
      - Search
  /template/{layoutId}:
    post:
      summary: Add a template from a Layout
      description: Use the provided layout as a base for a new template
      operationId: template.add.from.layout
      x-api-path-slug: templatelayoutid-post
      parameters:
      - in: formData
        name: description
        description: A description of the Template
      - in: formData
        name: includeWidgets
        description: Flag indicating whether to include the widgets in the Template
      - in: path
        name: layoutId
        description: The Layout ID
      - in: formData
        name: name
        description: The Template Name
      - in: formData
        name: tags
        description: Comma separated list of Tags for the template
      responses:
        200:
          description: OK
      tags:
      - Template
      - From
      - Layout
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