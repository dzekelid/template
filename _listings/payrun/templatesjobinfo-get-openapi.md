---
swagger: "2.0"
x-collection-name: PayRun
x-complete: 0
info:
  title: Pay Run.IO Gets the job info template
  description: Return the job info data object template
  version: 17.18.6.206
host: api.test.payrun.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Templates/address:
    get:
      summary: Gets the address template
      description: Return the address data object template
      operationId: GetAddressTemplate
      x-api-path-slug: templatesaddress-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Address
      - Template
  /Templates/applicationinfo:
    get:
      summary: Gets the application info template
      description: Return the application info data object template
      operationId: GetApplicationInfoTemplate
      x-api-path-slug: templatesapplicationinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Application
      - Info
      - Template
  /Templates/bankaccount:
    get:
      summary: Gets the bank account template
      description: Return the bank account data object template
      operationId: GetBankAccountTemplate
      x-api-path-slug: templatesbankaccount-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Bank
      - Account
      - Template
  /Templates/benefitpayinstruction:
    get:
      summary: Gets the benefit pay instruction template
      description: Return the benefit pay instruction data object template
      operationId: GetBenefitPayInstructionTemplate
      x-api-path-slug: templatesbenefitpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Benefit
      - Pay
      - Instruction
      - Template
  /Templates/benefitytdpayinstruction:
    get:
      summary: Gets the benefit YTD pay instruction template
      description: Return the benefit YTD pay instruction data object template
      operationId: GetBenefitYtdPayInstructionTemplate
      x-api-path-slug: templatesbenefitytdpayinstruction-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Benefit
      - YTD
      - Pay
      - Instruction
      - Template
  /Templates/commentary:
    get:
      summary: Gets the commentary template
      description: Return the commentary data object template
      operationId: GetCommentaryTemplate
      x-api-path-slug: templatescommentary-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Commentary
      - Template
  /Templates/employee:
    get:
      summary: Gets the employee template
      description: Return the employee data object template
      operationId: GetEmployeeTemplate
      x-api-path-slug: templatesemployee-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Template
  /Templates/employeepartner:
    get:
      summary: Gets the employee partner template
      description: Return the employee partner data object template
      operationId: GetEmployeePartnerTemplate
      x-api-path-slug: templatesemployeepartner-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employee
      - Partner
      - Template
  /Templates/employer:
    get:
      summary: Gets the employer template
      description: Return the employer data object template
      operationId: GetEmployerTemplate
      x-api-path-slug: templatesemployer-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Employer
      - Template
  /Templates/errormodel:
    get:
      summary: Gets the error model template
      description: Return the error model data object template
      operationId: GetErrorModelTemplate
      x-api-path-slug: templateserrormodel-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Error
      - Model
      - Template
  /Templates/hmrcsettings:
    get:
      summary: Gets the hmrc settings template
      description: Return the hmrc settings data object template
      operationId: GetHmrcSettingsTemplate
      x-api-path-slug: templateshmrcsettings-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Hmrc
      - Settings
      - Template
  /Templates/jobinfo:
    get:
      summary: Gets the job info template
      description: Return the job info data object template
      operationId: GetJobInfoTemplate
      x-api-path-slug: templatesjobinfo-get
      parameters:
      - in: header
        name: Api-Version
        description: The version of the api to target
      - in: header
        name: Authorization
        description: The OAuth 1 authorization header
      responses:
        200:
          description: OK
      tags:
      - Job
      - Info
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