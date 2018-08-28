{
  "info": {
    "name": "Dezrez Deletes a Letter Template",
    "_postman_id": "9f138342-075a-4aeb-86e7-e4c88a3db085",
    "description": "Deletes a letter template.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "S",
      "item": [
        {
          "id": "be5da7d8-d206-4ec1-9a12-07942249ba33",
          "name": "DocumentGeneration_DeleteLetterTemplateByidByuseageLimit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/documentgeneration/deletelettertemplate/:id/:useageLimit"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "useageLimit",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a letter template."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f76089b2-78aa-49c0-b75f-f88185783bc1"
            }
          ]
        }
      ]
    }
  ]
}