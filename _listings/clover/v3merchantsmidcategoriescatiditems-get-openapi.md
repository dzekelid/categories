---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get all items in a single category
  version: 1.0.0
  description: Get all items in a single category.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/order_type_categories:
    post:
      summary: Create or delete a order type category
      description: Create or delete a order type category.
      operationId: CreateOrDeleteOrderTypeCategories
      x-api-path-slug: v3merchantsmidorder-type-categories-post
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Order
      - Type
      - Categories
  /v3/merchants/{mId}/categories:
    get:
      summary: Get all categories
      description: Categories alter the user experience of the Register app. Items
        will appear in the Register app within the categories they are members of.
        Items may be associated with no, one or multiple categories. Items are displayed
        in Register in the order in which they are added to a category. Categories
        are displayed in Register using the sort order value for each category.
      operationId: GetCategories
      x-api-path-slug: v3merchantsmidcategories-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, sortOrder, name, id]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
    post:
      summary: Create an item category
      description: Create an item category.
      operationId: CreateCategory
      x-api-path-slug: v3merchantsmidcategories-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
  /v3/merchants/{mId}/categories/{catId}:
    get:
      summary: Get a category
      description: Get a category.
      operationId: GetCategory
      x-api-path-slug: v3merchantsmidcategoriescatid-get
      parameters:
      - in: path
        name: catId
        description: Category Id
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
    post:
      summary: Update a category
      description: Update a category.
      operationId: UpdateCategory
      x-api-path-slug: v3merchantsmidcategoriescatid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catId
        description: Category Id
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
    delete:
      summary: Delete a single item category
      description: Delete a single item category.
      operationId: DeleteCategory
      x-api-path-slug: v3merchantsmidcategoriescatid-delete
      parameters:
      - in: path
        name: catId
        description: Category Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
  /v3/merchants/{mId}/categories/{catId}/items:
    get:
      summary: Get all items in a single category
      description: Get all items in a single category.
      operationId: GetCategoryItems
      x-api-path-slug: v3merchantsmidcategoriescatiditems-get
      parameters:
      - in: path
        name: catId
        description: Category Id
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, sortOrder, name, id]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Categories
      - CatId
      - Items
  /v3/merchants/{mId}/items/{itemId}/categories:
    get:
      summary: Get all categories of a single item
      description: Get all categories of a single item.
      operationId: GetItemCategories
      x-api-path-slug: v3merchantsmiditemsitemidcategories-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: query
        name: filter
        description: 'Filter fields: [modifiedTime, deleted, sortOrder, name, id]'
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Items
      - ItemId
      - Categories
  /v3/merchants/{mId}/category_items:
    post:
      summary: Create or delete an item/category association
      description: Create or delete an item/category association.
      operationId: CreateOrDeleteCategoryItems
      x-api-path-slug: v3merchantsmidcategory-items-post
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [items]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Category
      - Items
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