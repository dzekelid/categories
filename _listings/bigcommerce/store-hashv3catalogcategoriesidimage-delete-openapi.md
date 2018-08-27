---
swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 0
info:
  title: BigCommerce Delete a category image
  description: ""
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/categories:
    get:
      summary: Retrieve categories
      description: Returns a paginated categories collection from the BigCommerce
        Catalog
      operationId: V3CatalogCategoriesByStoreHashGet
      x-api-path-slug: store-hashv3catalogcategories-get
      parameters:
      - in: query
        name: is_visible
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Categories
    delete:
      summary: Delete a category or categories
      description: ""
      operationId: V3CatalogCategoriesByStoreHashDelete
      x-api-path-slug: store-hashv3catalogcategories-delete
      parameters:
      - in: query
        name: is_visible
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Category
      - Categories
    post:
      summary: Create a new category
      description: ""
      operationId: V3CatalogCategoriesByStoreHashPost
      x-api-path-slug: store-hashv3catalogcategories-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - New
      - Category
  /{store_hash}/v3/catalog/categories/{id}:
    get:
      summary: Retrieve a single category
      description: ""
      operationId: V3CatalogCategoriesByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogcategoriesid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Single
      - Category
    put:
      summary: Update a category
      description: Update a `Category` in the BigCommerce Catalog
      operationId: V3CatalogCategoriesByStoreHashAndIdPut
      x-api-path-slug: store-hashv3catalogcategoriesid-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Category
    delete:
      summary: Delete a single category
      description: ""
      operationId: V3CatalogCategoriesByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogcategoriesid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Category
  /{store_hash}/v3/catalog/categories/{id}/image:
    post:
      summary: Create an image for a category
      description: ""
      operationId: V3CatalogCategoriesImageByStoreHashAndIdPost
      x-api-path-slug: store-hashv3catalogcategoriesidimage-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Imagea
      - Category
    delete:
      summary: Delete a category image
      description: ""
      operationId: V3CatalogCategoriesImageByStoreHashAndIdDelete
      x-api-path-slug: store-hashv3catalogcategoriesidimage-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Category
      - Image
  /{store_hash}/v3/catalog/categories/tree:
    get:
      summary: Retrieve category structure/tree
      description: ""
      operationId: V3CatalogCategoriesTreeByStoreHashGet
      x-api-path-slug: store-hashv3catalogcategoriestree-get
      parameters:
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - Category
      - Structure
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