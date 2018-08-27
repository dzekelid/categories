{
  "info": {
    "name": "reverb Get Csps Categories",
    "_postman_id": "8d19862d-bdb8-42a8-bee6-a2758fe592f2",
    "description": "Get csps categories.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Categories",
      "item": [
        {
          "id": "013c3c84-ea31-4536-b15c-900e0dffd120",
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
              "id": "96614dae-0a4f-4b04-9e91-74478f46fa16"
            }
          ]
        },
        {
          "id": "5948462a-c1a3-4a5c-91ba-ff3d62c2fff0",
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
              "id": "3f56c94b-c922-4c08-8181-ef45efa3d984"
            }
          ]
        },
        {
          "id": "1bbcb914-271c-49c7-9d6d-b8c5a501abcc",
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
              "id": "952a7351-3554-4413-999e-e604bef198dd"
            }
          ]
        },
        {
          "id": "9ece4ac5-e3c4-463e-b7c3-620fbfe10a11",
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
              "id": "e845a645-b339-47a7-91f2-04041398c1dc"
            }
          ]
        },
        {
          "id": "582c377f-cc26-4e74-b468-f9f5353c8978",
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
              "id": "b6092062-6c6b-4c66-8a79-523dbc261ad2"
            }
          ]
        }
      ]
    },
    {
      "name": "Csps",
      "item": [
        {
          "id": "093931c6-2315-4b38-aa77-130e5a01e411",
          "name": "getCspsCategories",
          "request": {
            "url": "http://api.reverb.com/api/csps/categories",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get csps categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88b39f24-d916-4c8d-ac3e-21038ffec37a"
            }
          ]
        }
      ]
    }
  ]
}