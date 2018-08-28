{
  "info": {
    "name": "Pay Run.IO Gets the hmrc settings template",
    "_postman_id": "b40eb0ff-4adf-4144-ab5c-397e3f8cb4a0",
    "description": "Return the hmrc settings data object template",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "HmrcSettings",
      "item": [
        {
          "id": "9c8e67bb-2f8b-4f44-b7bd-320d85570240",
          "name": "GetHmrcSettingsSchema",
          "request": {
            "url": "http://api.test.payrun.io/Schemas/HmrcSettings.xsd",
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the HmrcSettings schema object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4517d145-44db-4e37-86c9-b7af595dcbc6"
            }
          ]
        }
      ]
    },
    {
      "name": "Hmrc",
      "item": [
        {
          "id": "cb57a90a-bf3b-4d16-9bef-def6a021f176",
          "name": "GetHmrcSettingsTemplate",
          "request": {
            "url": "http://api.test.payrun.io/Templates/hmrcsettings",
            "method": "GET",
            "header": [
              {
                "key": "Api-Version",
                "value": "{}",
                "description": "The version of the api to target",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "The OAuth 1 authorization header",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Return the hmrc settings data object template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b3692e7-6190-4af7-93c2-5f6f4d1f5052"
            }
          ]
        }
      ]
    }
  ]
}