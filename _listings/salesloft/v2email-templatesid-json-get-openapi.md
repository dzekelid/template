---
swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 0
info:
  title: SalesLoft Fetch an email template
  description: Fetches an email template, by ID only.
  version: v2
host: api.salesloft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/email_templates/{id}.json:
    get:
      summary: Fetch an email template
      description: Fetches an email template, by ID only.
      operationId: v2.email_templates.id.json.get
      x-api-path-slug: v2email-templatesid-json-get
      parameters:
      - in: path
        name: id
        description: EmailTemplate ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Email
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