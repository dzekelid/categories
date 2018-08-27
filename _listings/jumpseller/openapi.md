swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
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
    get:
      summary: Get Customer Categories
      description: Retrieve a single customercategory..
      operationId: getCustomerCategories.json
      x-api-path-slug: customer-categoriesid-json-get
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
    put:
      summary: Put Customer Categories
      description: Update a customercategory..
      operationId: putCustomerCategories.json
      x-api-path-slug: customer-categoriesid-json-put
      parameters:
      - in: body
        name: body
        description: CustomerCategory parameters
        schema:
          $ref: '#/definitions/holder'
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
  /customer_categories/{id}/customers.json:
    delete:
      summary: Delete Customer Categories Customers
      description: Delete customers from an existing customercategory..
      operationId: deleteCustomerCategoriesCustomers.json
      x-api-path-slug: customer-categoriesidcustomers-json-delete
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
      - Customers
      - Json
    get:
      summary: Get Customer Categories Customers
      description: Retrieves the customers in a customercategory..
      operationId: getCustomerCategoriesCustomers.json
      x-api-path-slug: customer-categoriesidcustomers-json-get
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
      - Customers
      - Json
    post:
      summary: Post Customer Categories Customers
      description: Adds customers to a customercategory..
      operationId: postCustomerCategoriesCustomers.json
      x-api-path-slug: customer-categoriesidcustomers-json-post
      parameters:
      - in: body
        name: body
        description: Customer parameters
        schema:
          $ref: '#/definitions/holder'
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
      - Customers
      - Json
  /products/category/{category_id}.json:
    get:
      summary: Get Products Category Category
      description: ""
      operationId: getProductsCategoryCategory.json
      x-api-path-slug: productscategorycategory-id-json-get
      parameters:
      - in: path
        name: category_id
        description: Category ID of the Product used as filter
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Products
      - Category
      - Category
      - Id
      - Json
  /products/category/{category_id}/count.json:
    get:
      summary: Get Products Category Category Count
      description: ""
      operationId: getProductsCategoryCategoryCount.json
      x-api-path-slug: productscategorycategory-idcount-json-get
      parameters:
      - in: path
        name: category_id
        description: Category ID of the Product used as filter
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Products
      - Category
      - Category
      - Id
      - Count
      - Json