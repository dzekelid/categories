---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Delete Customer Categories
  description: Delete an existing customercategory..
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /categories.json:
    get:
      summary: Get Categories
      description: Retrieve all categories..
      operationId: getCategories.json
      x-api-path-slug: categories-json-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Json
    post:
      summary: Post Categories
      description: Create a new category..
      operationId: postCategories.json
      x-api-path-slug: categories-json-post
      parameters:
      - in: body
        name: body
        description: Category parameters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Json
  /categories/{id}.json:
    delete:
      summary: Delete Categories
      description: Delete an existing category..
      operationId: deleteCategories.json
      x-api-path-slug: categoriesid-json-delete
      parameters:
      - in: path
        name: id
        description: Id of the Category
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Id
      - Json
    get:
      summary: Get Categories
      description: Retrieve a single category..
      operationId: getCategories.json
      x-api-path-slug: categoriesid-json-get
      parameters:
      - in: path
        name: id
        description: Id of the Category
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Id
      - Json
    put:
      summary: Put Categories
      description: Modify an existing category..
      operationId: putCategories.json
      x-api-path-slug: categoriesid-json-put
      parameters:
      - in: body
        name: body
        description: Category parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Id of the Category
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Categories
      - Id
      - Json
  /customer_categories.json:
    get:
      summary: Get Customer Categories
      description: Retrieve all customer categories..
      operationId: getCustomerCategories.json
      x-api-path-slug: customer-categories-json-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Categories
      - Json
    post:
      summary: Post Customer Categories
      description: Create a new customercategory..
      operationId: postCustomerCategories.json
      x-api-path-slug: customer-categories-json-post
      parameters:
      - in: body
        name: body
        description: CustomerCategory parameters
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Categories
      - Json
  /customer_categories/{id}.json:
    delete:
      summary: Delete Customer Categories
      description: Delete an existing customercategory..
      operationId: deleteCustomerCategories.json
      x-api-path-slug: customer-categoriesid-json-delete
      parameters:
      - in: path
        name: id
        description: Id of the CustomerCategory
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Customer
      - Categories
      - Id
      - Json
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