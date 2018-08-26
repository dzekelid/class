{
  "info": {
    "name": "Plentymarkets Get a contact class",
    "_postman_id": "d2ccc690-2e27-4470-a7f2-66b254bd37c3",
    "description": "Gets a contact class. The ID of the contact class must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Contact",
      "item": [
        {
          "id": "fea208dc-79b3-44ac-a50b-5bddd3f14cd8",
          "name": "getRestAccountsContactsClassesContactclass",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/contacts/classes/:contactClassId"
              ],
              "variable": [
                {
                  "id": "contactClassId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets a contact class. The ID of the contact class must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01063058-13ee-4381-9a15-4fab075fefda"
            }
          ]
        }
      ]
    }
  ]
}