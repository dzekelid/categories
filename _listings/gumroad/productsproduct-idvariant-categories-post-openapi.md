---
swagger: "2.0"
x-collection-name: Gumroad
x-complete: 0
info:
  title: Gumroad Post Products Variant Categories
  description: Create a new variant category on a product.
  termsOfService: https://gumroad.com/terms
  version: v1
host: api.gumroad.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /products/:product_id/variant_categories:
    get:
      summary: Get Products Variant Categories
      description: Retrieve all of the existing variant categories of a product.
      operationId: getProductsProductVariantCategories
      x-api-path-slug: productsproduct-idvariant-categories-get
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
    post:
      summary: Post Products Variant Categories
      description: Create a new variant category on a product.
      operationId: postProductsProductVariantCategories
      x-api-path-slug: productsproduct-idvariant-categories-post
      parameters:
      - in: query
        name: title
      - in: query
        name: variant_category
      responses:
        200:
          description: OK
      tags:
      - Products
      - Variant
      - Categories
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---