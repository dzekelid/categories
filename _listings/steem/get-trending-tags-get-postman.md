{
  "info": {
    "name": "Steem get trending categories",
    "_postman_id": "e7e19002-04e7-4949-b0fb-a2cda38478a6",
    "description": "get tags",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "ffa7c0b3-8cff-4b24-9624-a0b823693f9e",
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
              "id": "d3e2a88f-2b7a-4793-808c-d20ec2096217"
            }
          ]
        },
        {
          "id": "f0aaf40c-652d-42e8-8aca-0c1e746ea545",
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
              "id": "86420200-e8e6-47e5-a00d-c97f2edbdb1b"
            }
          ]
        },
        {
          "id": "5b44f1f6-b9ce-41ea-9f39-7334b8f119a7",
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
              "id": "31c0ed73-ab50-4af1-b5b5-d9124b1cffe4"
            }
          ]
        },
        {
          "id": "2d8ef39c-b3e9-4554-bf8e-e96df7067875",
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
              "id": "200de05f-94a4-48ea-be69-4e77497b9e16"
            }
          ]
        },
        {
          "id": "96faf05a-e329-49b2-9bb1-815d81bfb99c",
          "name": "get-tags",
          "request": {
            "url": "http://api.steemjs.com/get_trending_tags?afterTag=%7B%7D&limit=%7B%7D",
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
              "id": "47c02b7c-6867-4a01-83d3-e5ea8cecf333"
            }
          ]
        }
      ]
    }
  ]
}