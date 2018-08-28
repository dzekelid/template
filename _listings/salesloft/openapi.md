swagger: "2.0"
x-collection-name: SalesLoft
x-complete: 1
info:
  title: SalesLoft
  description: salesloft-helps-transform-sales-teams-into-modern-sales-organizations---converting-more-target-accounts-into-customer-accounts
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
  /v2/team_templates/{id}.json:
    get:
      summary: Fetch a team template
      description: Fetches a team template, by ID only.
      operationId: v2.team_templates.id.json.get
      x-api-path-slug: v2team-templatesid-json-get
      parameters:
      - in: path
        name: id
        description: Team Template ID
      responses:
        200:
          description: OK
      tags:
      - Sales
      - Fetch
      - Team
      - Template