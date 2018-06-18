---
swagger: "2.0"
x-collection-name: Digital River
x-complete: 1
info:
  title: Digital River Shopper API
  description: the-dr-connect-shopper-api-operates-on-a-store-and-products-that-are-set-up-in-global-commerce--
  version: v1
host: store.digitalriver.com
basePath: /store/{mysite}
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/shoppers/me/categories:
    get:
      summary: Get Shoppers Me Categories
      description: Get shoppers me categories.
      operationId: getV1ShoppersMeCategories
      x-api-path-slug: v1shoppersmecategories-get
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Categories
  /v1/shoppers/me/categories/{id}:
    get:
      summary: Get Shoppers Me Categories
      description: Get shoppers me categories.
      operationId: getV1ShoppersMeCategories
      x-api-path-slug: v1shoppersmecategoriesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Categories
  /v1/shoppers/me/categories/{id}/products:
    get:
      summary: Get Shoppers Me Categories Products
      description: Get shoppers me categories products.
      operationId: getV1ShoppersMeCategoriesProducts
      x-api-path-slug: v1shoppersmecategoriesidproducts-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Shoppers
      - Me
      - Categories
      - Products
---