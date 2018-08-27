{
  "info": {
    "name": "Icon Finder List all categories",
    "_postman_id": "77f0decb-852d-41c3-9e93-65df1877d408",
    "description": "List all categories sorted ascendingly by their identifier.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "e6d81657-f6dc-4afb-aea2-d05e54525541",
          "name": "getCategories",
          "request": {
            "url": "http://api.iconfinder.com/v2/categories?after=%7B%7D&count=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all categories sorted ascendingly by their identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b93f1e29-d4be-40d6-b4fe-86996430d462"
            }
          ]
        }
      ]
    }
  ]
}