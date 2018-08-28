---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Mail Settings Template
  description: "**This endpoint allows you to retrieve your current legacy email template
    settings.**\n\nThis setting refers to our original email templates. We currently
    support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
    \n\nThe legacy email template setting wraps an HTML template around your email
    content. This can be useful for sending out marketing email and/or other HTML
    formatted messages.\n\nMail settings allow you to tell SendGrid specific things
    to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
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