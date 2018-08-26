{
  "info": {
    "name": "Steem get trending categories",
    "_postman_id": "cc7fe96f-8a52-4c5d-be3b-00a1a9568faf",
    "description": "get tags",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "a2ec40fc-4569-4c53-ba6f-88a63f0220fc",
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
              "id": "8f6b98f3-704a-458f-be7b-abb04e4376f8"
            }
          ]
        },
        {
          "id": "ec56197f-fbdc-4707-801a-0306677b9696",
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
              "id": "849b0c22-571c-44dc-bf05-67a78a47c4ca"
            }
          ]
        },
        {
          "id": "73451a98-3f25-42c5-872d-538b71956fd8",
          "name": "get-tags2",
          "request": {
            "url": "http://api.steemjs.com/get_recent_categories?after=%7B%7D&limit=%7B%7D",
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
              "id": "99347719-7fff-4b33-9472-8006c62cd8ff"
            }
          ]
        },
        {
          "id": "7ff9341c-dfb9-4e34-a6ed-9b2e6f6f58cc",
          "name": "get-tags3",
          "request": {
            "url": "http://api.steemjs.com/get_trending_categories?after=%7B%7D&limit=%7B%7D",
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
              "id": "a00b5e47-2c02-487d-a93a-f84d174f26f4"
            }
          ]
        }
      ]
    }
  ]
}