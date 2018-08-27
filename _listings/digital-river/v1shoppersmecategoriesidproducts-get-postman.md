{
  "info": {
    "name": "Digital River Shopper API Get Shoppers Me Categories Products",
    "_postman_id": "8ed3cbba-53d4-46d6-a597-3fb2b5ca33c6",
    "description": "Get shoppers me categories products.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shoppers",
      "item": [
        {
          "id": "8d118b1c-e276-4268-8785-31a9c992ec80",
          "name": "getV1ShoppersMeCategories",
          "request": {
            "url": "http://store.digitalriver.com/store/TODO Add Value for parameter.../v1/shoppers/me/categories",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0dfb64b0-e88f-4bd0-bf16-aaee4c847800"
            }
          ]
        },
        {
          "id": "2d4fa67c-e253-4167-8a4f-d8058af210b5",
          "name": "getV1ShoppersMeCategories",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/categories/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f046df46-6a1f-4df1-bc9e-c219990603cd"
            }
          ]
        },
        {
          "id": "1c4b6188-8b8a-4f9f-9bc5-4f26198e55f8",
          "name": "getV1ShoppersMeCategoriesProducts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "store.digitalriver.com",
              "path": [
                "store",
                "TODO%20Add%20Value%20for%20parameter...",
                "v1/shoppers/me/categories/:id/products"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get shoppers me categories products."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f29ebc9-9c30-4ae9-bf6c-a960edbc8e2e"
            }
          ]
        }
      ]
    }
  ]
}