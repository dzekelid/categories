---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Get Categories Uu
  description: Get category details
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /categories:
    get:
      summary: Get Categories
      description: List of supported product categories
      operationId: getCategories
      x-api-path-slug: categories-get
      responses:
        200:
          description: OK
      tags:
      - Categories
  /categories/flat:
    get:
      summary: Get Categories Flat
      description: Get categories flat.
      operationId: getCategoriesFlat
      x-api-path-slug: categoriesflat-get
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Flat
  /categories/taxonomy:
    get:
      summary: Get Categories Taxonomy
      description: Full taxonomy tree of categories including middle categories
      operationId: getCategoriesTaxonomy
      x-api-path-slug: categoriestaxonomy-get
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Taxonomy
  /categories/{product_type}/{category}:
    get:
      summary: Get Categories Product Type Category
      description: Get categories product type category.
      operationId: getCategoriesProductTypeCategory
      x-api-path-slug: categoriesproduct-typecategory-get
      parameters:
      - in: path
        name: category
      - in: path
        name: product_type
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Product
      - Type
      - Category
  /categories/{uuid}:
    get:
      summary: Get Categories Uu
      description: Get category details
      operationId: getCategoriesUu
      x-api-path-slug: categoriesuuid-get
      parameters:
      - in: path
        name: uuid
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Uuid
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