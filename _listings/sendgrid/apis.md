---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Template
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid - Get Mail Settings Template
  x-api-slug: mail-settingstemplate-get
  description: "**This endpoint allows you to retrieve your current legacy email template
    settings.**\n\nThis setting refers to our original email templates. We currently
    support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
    \n\nThe legacy email template setting wraps an HTML template around your email
    content. This can be useful for sending out marketing email and/or other HTML
    formatted messages.\n\nMail settings allow you to tell SendGrid specific things
    to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/mail-settingstemplate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/mail-settingstemplate-get-openapi.md
- name: SendGrid - Patch Mail Settings Template
  x-api-slug: mail-settingstemplate-patch
  description: "**This endpoint allows you to update your current legacy email template
    settings.**\n\nThis setting refers to our original email templates. We currently
    support more fully featured [transactional templates](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
    \n\nThe legacy email template setting wraps an HTML template around your email
    content. This can be useful for sending out marketing email and/or other HTML
    formatted messages.\n\nMail settings allow you to tell SendGrid specific things
    to do to every email that you send to your recipients over SendGrid???s [Web API](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
    or [SMTP Relay](https://sendgrid.com/docs/API_Reference/SMTP_API/index.html)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/mail-settingstemplate-patch-openapi.md
- name: SendGrid - Delete Templates Template
  x-api-slug: templatestemplate-id-delete
  description: |-
    **This endpoint allows you to delete a transactional template.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-id-delete-openapi.md
- name: SendGrid - Get Templates Template
  x-api-slug: templatestemplate-id-get
  description: |-
    **This endpoint allows you to retrieve a single transactional template.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-id-get-openapi.md
- name: SendGrid - Patch Templates Template
  x-api-slug: templatestemplate-id-patch
  description: |-
    **This endpoint allows you to edit a transactional template.**

    Each user can create up to 300 different transactional templates. Transactional templates are specific to accounts and subusers. Templates created on a parent account will not be accessible from the subuser accounts.

    Transactional templates are templates created specifically for transactional email and are not to be confused with [Marketing Campaigns templates](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/templates.html). For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-id-patch-openapi.md
- name: SendGrid - Add Templates Template  Versions
  x-api-slug: templatestemplate-idversions-post
  description: |-
    **This endpoint allows you to create a new version of a template.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-idversions-post-openapi.md
- name: SendGrid - Delete Templates Template  Versions Version
  x-api-slug: templatestemplate-idversionsversion-id-delete
  description: |-
    **This endpoint allows you to delete one of your transactional template versions.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string | The ID of the template version |
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-idversionsversion-id-delete-openapi.md
- name: SendGrid - Get Templates Template  Versions Version
  x-api-slug: templatestemplate-idversionsversion-id-get
  description: |-
    **This endpoint allows you to retrieve a specific version of a template.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string |  The ID of the template version |
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-idversionsversion-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-idversionsversion-id-get-openapi.md
- name: SendGrid - Patch Templates Template  Versions Version
  x-api-slug: templatestemplate-idversionsversion-id-patch
  description: |-
    **This endpoint allows you to edit a version of one of your transactional templates.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.

    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string | The ID of the template version |
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-idversionsversion-id-patch-openapi.md
- name: SendGrid - Add Templates Template  Versions Version  Activate
  x-api-slug: templatestemplate-idversionsversion-idactivate-post
  description: |-
    **This endpoint allows you to activate a version of one of your templates.**

    Each transactional template can have multiple versions, each version with its own subject and content. Each user can have up to 300 versions across across all templates.


    For more information about transactional templates, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Transactional_Templates/index.html).

    ## URI Parameters
    | URI Parameter | Type | Description |
    |---|---|---|
    | template_id | string | The ID of the original template |
    | version_id | string |  The ID of the template version |
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/template/master/_listings/sendgrid/templatestemplate-idversionsversion-idactivate-post-openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-api-gallery
  url: http://school.digger.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sendgrid.stack.network
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---