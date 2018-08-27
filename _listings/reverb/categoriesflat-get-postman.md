{
  "info": {
    "name": "reverb Get Categories Flat",
    "_postman_id": "0aacf6ed-bd97-45b3-af3d-f1ae1e0c9f8a",
    "description": "Get categories flat.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "56ee8f94-cd31-4f97-a92f-52facc3c6271",
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
              "id": "b0f73a47-8eb6-479c-9adc-33da521fc336"
            }
          ]
        },
        {
          "id": "ebaf880d-37cc-4163-90e5-ad7e3b61d89f",
          "name": "getCategoriesFlat",
          "request": {
            "url": "http://api.reverb.com/api/categories/flat",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get categories flat."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e3fc0872-7f0d-454d-b5af-040af2565f26"
            }
          ]
        }
      ]
    }
  ]
}