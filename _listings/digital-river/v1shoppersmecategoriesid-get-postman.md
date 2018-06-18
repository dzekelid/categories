{
  "info": {
    "name": "Digital River Shopper API Get Shoppers Me Categories",
    "_postman_id": "04e50370-ccdc-4418-81ff-8849fdf9dad2",
    "description": "Get shoppers me categories.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shoppers",
      "item": [
        {
          "id": "0967d23f-6a99-4305-83a8-3498332140ce",
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
              "id": "ef6815da-bfe8-4a0a-a183-c57fc6b532d0"
            }
          ]
        },
        {
          "id": "c2e98d81-7bca-49d2-a331-ed8fe5c93374",
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
              "id": "d7a36512-bf18-48fa-88f8-c185d60bbf5d"
            }
          ]
        }
      ]
    }
  ]
}