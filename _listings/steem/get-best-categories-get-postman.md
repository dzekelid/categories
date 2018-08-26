{
  "info": {
    "name": "Steem get best categories",
    "_postman_id": "a4f3aa98-12d0-405e-877b-fa2546ff3401",
    "description": "get tags",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "dfa86f3a-b7e5-4a98-95ca-752945f568be",
          "name": "get-tags",
          "request": {
            "url": "http://api.steemjs.com/get_active_categories?after=%7B%7D&limit=%7B%7D",
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
            "description": "get tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c6b1be6-8d2e-48d0-b992-1fa7a71beca9"
            }
          ]
        },
        {
          "id": "4651bfc4-e432-4058-8f8e-e5691960ad24",
          "name": "get-tags1",
          "request": {
            "url": "http://api.steemjs.com/get_best_categories?after=%7B%7D&limit=%7B%7D",
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
            "description": "get tags"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67d919bd-ccb7-4ee6-a1d7-e3ed48200526"
            }
          ]
        }
      ]
    }
  ]
}