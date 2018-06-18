{
  "info": {
    "name": "Crunch Base Get Categories",
    "_postman_id": "21bb7ce1-1e07-47eb-a4ce-f81c778f0049",
    "description": "Get Categories",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "db2d3851-1136-4f24-b250-02f7647adb5f",
          "name": "categories",
          "request": {
            "url": "http://api.crunchbase.com/v/3/categories?page=%7B%7D&sort_order=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbeaf6de-22ad-43fd-ac13-72ad92515c31"
            }
          ]
        }
      ]
    }
  ]
}