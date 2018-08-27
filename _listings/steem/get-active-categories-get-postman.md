{
  "info": {
    "name": "Steem get active categories",
    "_postman_id": "db15b950-7252-44f8-a932-c1f2da604590",
    "description": "get tags",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Get",
      "item": [
        {
          "id": "788bd841-f6ab-436e-b19e-b2c117180390",
          "name": "get-active-witnesses",
          "request": {
            "url": "http://api.steemjs.com/get_active_witnesses",
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
            "description": "get_active_witnesses"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62a4a8fb-55c4-4bac-9bdf-24756e8b4d4b"
            }
          ]
        },
        {
          "id": "56e003dd-d11e-428f-8bb2-3344c0ccd1ed",
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
              "id": "4a37d762-43ce-4b32-a124-87168d8de14d"
            }
          ]
        }
      ]
    }
  ]
}