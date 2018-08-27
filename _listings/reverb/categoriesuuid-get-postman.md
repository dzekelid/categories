{
  "info": {
    "name": "reverb Get Categories Uu",
    "_postman_id": "57890197-9bae-4de2-b323-44bebf3b2622",
    "description": "Get category details",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "932291fe-e4a8-47d5-b487-57cec75e4680",
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
              "id": "cb3f08f1-b99e-4c20-a827-5107f79e099f"
            }
          ]
        },
        {
          "id": "76a15da5-ba44-44fb-a518-0f7aef4ef024",
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
              "id": "4004c44f-21e9-411d-ae77-4b44735a0333"
            }
          ]
        },
        {
          "id": "3fae0e60-9ada-49b3-8c0e-37477cd17bc7",
          "name": "getCategoriesTaxonomy",
          "request": {
            "url": "http://api.reverb.com/api/categories/taxonomy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Full taxonomy tree of categories including middle categories"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ad5fc16-ead8-4cd9-b4ea-b07d37630e19"
            }
          ]
        },
        {
          "id": "d9aa9306-1fdd-4e92-955a-55fdf3c9d6ad",
          "name": "getCategoriesProductTypeCategory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "categories/:product_type/:category"
              ],
              "variable": [
                {
                  "id": "category",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "product_type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get categories product type category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31277447-f157-405d-bc38-7e04aa542ccd"
            }
          ]
        },
        {
          "id": "709a5640-055e-47ad-b36e-d5857d640c73",
          "name": "getCategoriesUu",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reverb.com",
              "path": [
                "api",
                "categories/:uuid"
              ],
              "variable": [
                {
                  "id": "uuid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get category details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38a6186b-5def-4105-a835-938a7ded6981"
            }
          ]
        }
      ]
    }
  ]
}