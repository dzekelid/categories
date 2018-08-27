---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Get Categories Tree
  description: Get categories tree.
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/products/{productID}/relationships/categories:
    put:
      summary: Update Product <=> Categories Relationships
      description: Here you can update `Categories` to a product. `Categories` specified
        in the payload willbe related to the product any relatiosnhips to `Categories`
        **NOT** specified in payload will be removed.
      operationId: V2ProductsRelationshipsCategoriesByProductIDPut
      x-api-path-slug: v2productsproductidrelationshipscategories-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
    post:
      summary: Create Product <=> Categories Relationships
      description: Here you can add `Categories` to a product. `Categories` specified
        in the payload willbe related to the product.
      operationId: V2ProductsRelationshipsCategoriesByProductIDPost
      x-api-path-slug: v2productsproductidrelationshipscategories-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
    delete:
      summary: Delete Product <=> Categories Relationships
      description: Here you can delete a relationship between a `Product` and `Category`.
        Only relationships to `Categories` specified in the payload will be removed.
      operationId: V2ProductsRelationshipsCategoriesByProductIDDelete
      x-api-path-slug: v2productsproductidrelationshipscategories-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: productID
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Categories
      - Relationships
  /v2/categories:
    get:
      summary: Get Categories List
      description: Get categories list.
      operationId: V2CategoriesGet
      x-api-path-slug: v2categories-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Categories
      - List
  /v2/categories/tree:
    get:
      summary: Get Categories Tree
      description: Get categories tree.
      operationId: V2CategoriesTreeGet
      x-api-path-slug: v2categoriestree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Categories
      - Tree
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