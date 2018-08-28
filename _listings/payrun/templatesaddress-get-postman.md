{
  "info": {
    "name": "Pay Run.IO Gets the address template",
    "_postman_id": "5882c4ba-7892-4a4a-a08a-df9ff8a56c4a",
    "description": "Return the address data object template",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Address",
      "item": [
        {
          "id": "62371d6b-ce97-4b2b-b1f0-8439f14eb4ad",
          "name": "GetAddressTemplate",
          "request": {
            "url": "http://api.test.payrun.io/Templates/address",
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
            "description": "Return the address data object template"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae737738-c5be-4757-b84a-077f613eba9e"
            }
          ]
        }
      ]
    }
  ]
}