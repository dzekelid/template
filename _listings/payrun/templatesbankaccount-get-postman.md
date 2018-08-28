{
  "info": {
    "name": "Pay Run.IO Gets the bank account template",
    "_postman_id": "66fe1751-5370-44a0-af4b-f2163aca8abf",
    "description": "Return the bank account data object template",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "BankAccount",
      "item": [
        {
          "id": "980bb86a-c83e-4b48-ae6b-060b1b14164b",
          "name": "GetBankAccountSchema",
          "request": {
            "url": "http://api.test.payrun.io/Schemas/BankAccount.xsd",
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
            "description": "Returns the BankAccount schema object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50f05214-9745-47ee-9c6a-032a272ac113"
            }
          ]
        }
      ]
    },
    {
      "name": "Bank",
      "item": [
        {
          "id": "ed138a87-dbca-4c9d-9169-92203b450ba9",
          "name": "GetBankAccountTemplate",
          "request": {
            "url": "http://api.test.payrun.io/Templates/bankaccount",
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
            "description": "Return the bank account data object template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c6bb7fc-650d-4a42-811d-d99ce2296bf6"
            }
          ]
        }
      ]
    }
  ]
}