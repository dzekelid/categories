swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
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
    post:
      summary: Create a Category
      description: Create a category.
      operationId: V2CategoriesPost
      x-api-path-slug: v2categories-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
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
  /v2/categories/{categoryID}:
    get:
      summary: Get a Category
      description: Get a category.
      operationId: V2CategoriesByCategoryIDGet
      x-api-path-slug: v2categoriescategoryid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
    put:
      summary: Update a Category
      description: Update a category.
      operationId: V2CategoriesByCategoryIDPut
      x-api-path-slug: v2categoriescategoryid-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
    delete:
      summary: Delete a Category
      description: Delete a category.
      operationId: V2CategoriesByCategoryIDDelete
      x-api-path-slug: v2categoriescategoryid-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
  /v2/categories/{categoryID}/relationships/children:
    put:
      summary: Update Child Category Relationships
      description: Update child category relationships.
      operationId: V2CategoriesRelationshipsChildrenByCategoryIDPut
      x-api-path-slug: v2categoriescategoryidrelationshipschildren-put
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
    delete:
      summary: Delete Child Category Relationships
      description: Delete child category relationships.
      operationId: V2CategoriesRelationshipsChildrenByCategoryIDDelete
      x-api-path-slug: v2categoriescategoryidrelationshipschildren-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
  /categories/{categoryID}/relationships/children:
    post:
      summary: Create Child Category Relationships
      description: Create child category relationships.
      operationId: CategoriesRelationshipsChildrenByCategoryIDPost
      x-api-path-slug: categoriescategoryidrelationshipschildren-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Child
      - Category
      - Relationships
  /v2/categories/{parentCatID}/relationships/parent:
    put:
      summary: Update Parent Category Parent
      description: Update parent category parent.
      operationId: V2CategoriesRelationshipsParentByParentCatIDPut
      x-api-path-slug: v2categoriesparentcatidrelationshipsparent-put
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
        name: parentCatID
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Category
      - Parent
  /v2/categories/{categoryID}/relationships/categories:
    post:
      summary: Create Parent Category Relationship
      description: Using this endpoint you can create a relationship between a category
        and a parent category. When returning the category tree, you will see this
        relationship in place.
      operationId: V2CategoriesRelationshipsCategoriesByCategoryIDPost
      x-api-path-slug: v2categoriescategoryidrelationshipscategories-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Category
      - Relationship
  /categories/attributes:
    get:
      summary: Get Category Attributes
      description: Get category attributes.
      operationId: CategoriesAttributesGet
      x-api-path-slug: categoriesattributes-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
      - Attributes
  /v2/categories/{categoryID}/relationships/parent:
    delete:
      summary: Delete Parent Category Parent
      description: Delete parent category parent.
      operationId: V2CategoriesRelationshipsParentByCategoryIDDelete
      x-api-path-slug: v2categoriescategoryidrelationshipsparent-delete
      parameters:
      - in: header
        name: Accept
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Parent
      - Category
      - Parent
  /v2/categories/categories/tree:
    get:
      summary: Category Tree
      description: Category tree.
      operationId: V2CategoriesCategoriesTreeGet
      x-api-path-slug: v2categoriescategoriestree-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category
      - Tree
  /categories/{categoryID}/relationships/categories:
    delete:
      summary: Delete Category-Category Relationships
      description: Delete category-category relationships.
      operationId: CategoriesRelationshipsCategoriesByCategoryIDDelete
      x-api-path-slug: categoriescategoryidrelationshipscategories-delete
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryID
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Category-Category
      - Relationships