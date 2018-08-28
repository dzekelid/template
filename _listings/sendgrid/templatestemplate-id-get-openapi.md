---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Templates Template
  description: |-
    **This endpoint allows you to retrieve a single transactional template.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mail_settings/template:
    get:
      summary: Get Mail Settings Template
      description: "**This endpoint allows you to retrieve your current legacy email
        template settings.**\n\nThis setting refers to our original email templates.
        We currently support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
        \n\nThe legacy email template setting wraps an HTML template around your email
        content. This can be useful for sending out marketing email and/or other HTML
        formatted messages.\n\nMail settings allow you to tell SendGrid specific things
        to do to every email that you send to your recipients over SendGrid???s [Web
        API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.template.get
      x-api-path-slug: mail-settingstemplate-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Template
    patch:
      summary: Patch Mail Settings Template
      description: "**This endpoint allows you to update your current legacy email
        template settings.**\n\nThis setting refers to our original email templates.
        We currently support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
        \n\nThe legacy email template setting wraps an HTML template around your email
        content. This can be useful for sending out marketing email and/or other HTML
        formatted messages.\n\nMail settings allow you to tell SendGrid specific things
        to do to every email that you send to your recipients over SendGrid???s [Web
        API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html) or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
      operationId: mail_settings.template.patch
      x-api-path-slug: mail-settingstemplate-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Mail
      - Settings
      - Template
  /templates/{template_id}:
    delete:
      summary: Delete Templates Template
      description: |-
        **This endpoint allows you to delete a transactional template.**

        Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

        Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
      operationId: templates.template_id.delete
      x-api-path-slug: templatestemplate-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
      - Template
    get:
      summary: Get Templates Template
      description: |-
        **This endpoint allows you to retrieve a single transactional template.**

        Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

        Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
      operationId: templates.template_id.get
      x-api-path-slug: templatestemplate-id-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Templates
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