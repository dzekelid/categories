{
  "info": {
    "name": "reverb Get Categories",
    "_postman_id": "0124f13d-6f61-4601-8ade-39f9b9a3f6e6",
    "description": "List of supported product categories",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "817e2df0-71a3-4166-98ad-eba6263e095a",
          "name": "getCategories",
          "request": {
            "url": "http://api.reverb.com/api/categories",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of supported product categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37597348-8959-4ba6-a6db-37ec6e25e853"
            }
          ]
        }
      ]
    }
  ]
}