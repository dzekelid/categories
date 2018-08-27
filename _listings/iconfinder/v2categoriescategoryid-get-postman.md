{
  "info": {
    "name": "Icon Finder Get category details",
    "_postman_id": "2a8906cc-eeea-4fad-926e-7e4a73adf7e4",
    "description": "Get details about a specific category identified by its identifier.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "1a500b19-084b-4350-a164-cd470f08e98e",
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
              "id": "978217a2-5cb2-4a08-a0c8-c7ccd8bee79c"
            }
          ]
        },
        {
          "id": "2264634d-908f-4724-bc49-eecb6e913768",
          "name": "getV2CategoriesCategory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.iconfinder.com",
              "path": [
                "v2",
                "v2/categories/:categoryID"
              ],
              "variable": [
                {
                  "id": "categoryID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get details about a specific category identified by its identifier."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c358fb56-fef7-4d06-9143-c40526259d68"
            }
          ]
        }
      ]
    }
  ]
}