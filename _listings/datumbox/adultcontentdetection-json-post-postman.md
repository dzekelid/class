{
  "info": {
    "name": "Datumbox Classifies the Document as adult or noadult",
    "_postman_id": "08875e31-546e-47bc-9db3-008232884d8f",
    "description": "The Adult Content Detection function classifies the documents as adult or noadult based on their context. It can be used to detect whether a document contains content unsuitable for minors.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Adult Content",
      "item": [
        {
          "id": "286aa5cb-3221-458c-84c4-916cbcd34950",
          "name": "AdultContentDetection",
          "request": {
            "url": "http://api.datumbox.com/1.0/AdultContentDetection.json",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": "The text that you want to analyze"
                }
              ]
            },
            "description": "The Adult Content Detection function classifies the documents as adult or noadult based on their context. It can be used to detect whether a document contains content unsuitable for minors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23dd19f5-0e1b-4b22-833d-c8108fce78ad"
            }
          ]
        }
      ]
    }
  ]
}