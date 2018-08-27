---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Delete a default category link
  description: Deletes a link between a variation and a category that designates this
    category as the default category.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/categories:
    get:
      summary: List categories
      description: List categories.
      operationId: getRestCategories
      x-api-path-slug: restcategories-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: lang
        description: The languages of the category detail information
      - in: query
        name: level
        description: The level of the category
      - in: query
        name: linklist
        description: Filter for the linklist of categories
      - in: query
        name: name
        description: The name of the category
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: parentId
        description: The unique ID of the parent category
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      - in: query
        name: type
        description: The category type
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the detail information, the active clients (stores)
          list of the category and/or the linked Elmar category for each client
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
    post:
      summary: Creates new categories
      description: Creates new categories.
      operationId: postRestCategories
      x-api-path-slug: restcategories-post
      parameters:
      - in: body
        name: /rest/categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Creates
      - New
      - Categories
    put:
      summary: Updates categories
      description: Updates categories.
      operationId: putRestCategories
      x-api-path-slug: restcategories-put
      parameters:
      - in: body
        name: /rest/categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - S
      - Categories
  /rest/categories/{id}:
    get:
      summary: List categories
      description: List categories.
      operationId: getRestCategories
      x-api-path-slug: restcategoriesid-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category
      - in: path
        name: id
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: lang
        description: The languages of the category detail information
      - in: query
        name: level
        description: The level of the category
      - in: query
        name: linklist
        description: Filter for the linklist of categories
      - in: query
        name: name
        description: The name of the category
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: parentId
        description: The unique ID of the parent category
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      - in: query
        name: type
        description: The category type
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the detail information, the active clients (stores)
          list of the category and/or the linked Elmar category for each client
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
    delete:
      summary: Deletes a category
      description: Deletes a category. The ID of the category must be specified.
      operationId: deleteRestCategories
      x-api-path-slug: restcategoriesid-delete
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
    put:
      summary: Updates one category
      description: Updates an existing category. The ID of the category must be specified.
      operationId: putRestCategories
      x-api-path-slug: restcategoriesid-put
      parameters:
      - in: body
        name: /rest/categories/{id}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
  /rest/items/{id}/variations/{variationId}/variation_categories:
    get:
      summary: List categories linked to a variation
      description: Lists all categories linked to a variation.
      operationId: getRestItemsVariationsVariationVariationCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-categories-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
      - Linked
      - To
      - Variation
    post:
      summary: Link a category to a variation
      description: Creates a link between a category and a variation.
      operationId: postRestItemsVariationsVariationVariationCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-categories-post
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_categories
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Category
      - To
      - Variation
  /rest/markets/ebay/categories:
    get:
      summary: List categories
      description: Lists categories. By passing category ID as filter, only subcategories
        of that category will be returned. The marketplace ID filter is required.
      operationId: getRestMarketsEbayCategories
      x-api-path-slug: restmarketsebaycategories-get
      parameters:
      - in: query
        name: categoryId
        description: Filter that restricts the search result to categories that belong
          to the specified category ID
      - in: query
        name: marketplaceId
        description: Filter that restricts the search result to categories that belong
          to the specified marketplace ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
  /rest/markets/ebay/shop_categories:
    get:
      summary: List all eBay shop categories
      description: Lists all eBay shop categories.
      operationId: getRestMarketsEbayShopCategories
      x-api-path-slug: restmarketsebayshop-categories-get
      parameters:
      - in: query
        name: credentialsId
        description: The credentials ID for whom to fetch eBay shop categories
      - in: query
        name: viewType
        description: How should the eBay shop categories be returned
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - EBay
      - Shop
      - Categories
  /rest/categories/{categoryId}/documents:
    get:
      summary: List documents of a category
      description: Lists the documents of a category. The ID of the category must
        be specified.
      operationId: getRestCategoriesCategoryDocuments
      x-api-path-slug: restcategoriescategoryiddocuments-get
      parameters:
      - in: path
        name: categoryId
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Category
    post:
      summary: Upload category documents
      description: Uploads documents to a category. The ID of the category must be
        specified.
      operationId: postRestCategoriesCategoryDocuments
      x-api-path-slug: restcategoriescategoryiddocuments-post
      parameters:
      - in: body
        name: /rest/categories/{categoryId}/documents
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: categoryId
      - in: query
        name: directoryId
        description: The directory ID
      - in: query
        name: displayDate
        description: The date displayed on the document
      - in: query
        name: documents
        description: The array with the category documents
      - in: query
        name: number
        description: The document number
      - in: query
        name: numberWithPrefix
        description: Number with prefix
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Category
      - Documents
  /rest/categories/{categoryId}/documents/downloads:
    get:
      summary: Download category documents
      description: Downloads the documents of a category as a zip file. The ID of
        the category must be specified.
      operationId: getRestCategoriesCategoryDocumentsDownloads
      x-api-path-slug: restcategoriescategoryiddocumentsdownloads-get
      parameters:
      - in: path
        name: categoryId
      responses:
        200:
          description: OK
      tags:
      - Download
      - Category
      - Documents
  /rest/categories/{categoryId}/documents/{documentId}:
    delete:
      summary: Deletes a category document. The ID of the document must be specified.
      description: Deletes a category document. the id of the document must be specified..
      operationId: deleteRestCategoriesCategoryDocumentsDocument
      x-api-path-slug: restcategoriescategoryiddocumentsdocumentid-delete
      parameters:
      - in: path
        name: categoryId
      - in: path
        name: documentId
      responses:
        200:
          description: OK
      tags:
      - S
      - Category
      - Document
      - ""
      - ID
      - Of
      - Document
      - Must
      - Be
      - Specified
  /rest/categories/{id}/details:
    delete:
      summary: Delete category details for the specified languages
      description: Delete category details for the specified languages.
      operationId: deleteRestCategoriesDetails
      x-api-path-slug: restcategoriesiddetails-delete
      parameters:
      - in: body
        name: /rest/categories/{id}/details
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Detailsthe
      - Specified
      - Languages
  /rest/categories/{id}/templates:
    delete:
      summary: Delete a category template
      description: Deletes a category template. The ID of the category, the plenty
        ID of the client (store) and the language must be specified.
      operationId: deleteRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-delete
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
    get:
      summary: Get a category template
      description: Gets a category template. The ID of the category, the plenty ID
        of the client (store) and the language must be specified.
      operationId: getRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-get
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: lang
        description: The language of the template
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
    put:
      summary: Update a category template
      description: Updates a category template. The ID of the category, the plenty
        ID of the client (store) and the language must be specified.
      operationId: putRestCategoriesTemplates
      x-api-path-slug: restcategoriesidtemplates-put
      parameters:
      - in: body
        name: /rest/categories/{id}/templates
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Template
  /rest/category_branches:
    get:
      summary: Get category trees
      description: Get category trees.
      operationId: getRestCategoryBranches
      x-api-path-slug: restcategory-branches-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: type
        description: The category type
      responses:
        200:
          description: OK
      tags:
      - Category
      - Trees
  /rest/category_branches/{id}:
    get:
      summary: Get category tree
      description: Gets the category tree of a category. The ID of the category must
        be specified.
      operationId: getRestCategoryBranches
      x-api-path-slug: restcategory-branchesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
      - Tree
  /rest/items/variations/variation_categories:
    post:
      summary: Bulk create category links
      description: Creates up to 50 links between variations and categories. The ID
        of the variations and the ID of the categories must be specified.
      operationId: postRestItemsVariationsVariationCategories
      x-api-path-slug: restitemsvariationsvariation-categories-post
      parameters:
      - in: body
        name: /rest/items/variations/variation_categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Create
      - Category
      - Links
    put:
      summary: Bulk update category links
      description: Updates up to 50 links between variations and categories. The ID
        of the variations and the ID of the categories must be specified.
      operationId: putRestItemsVariationsVariationCategories
      x-api-path-slug: restitemsvariationsvariation-categories-put
      parameters:
      - in: body
        name: /rest/items/variations/variation_categories
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Bulk
      - Update
      - Category
      - Links
  /rest/items/{id}/variations/{variationId}/variation_categories/{catId}:
    delete:
      summary: Remove a category from a variation
      description: Deletes the link between a category and a variation.
      operationId: deleteRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-delete
      parameters:
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Category
      - From
      - Variation
    get:
      summary: Get link between category and variation
      description: Gets the link between a category and a variation.
      operationId: getRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-get
      parameters:
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Link
      - Between
      - Category
      - Variation
    put:
      summary: Update variation category link
      description: Updates the link between a category and a variation.
      operationId: putRestItemsVariationsVariationVariationCategoriesCat
      x-api-path-slug: restitemsidvariationsvariationidvariation-categoriescatid-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_categories/{catId}
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: catId
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Variation
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_default_categories:
    get:
      summary: List default category links
      description: Lists the default category of a variation for all clients (stores).
        The ID of the item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Default
      - Category
      - Links
    post:
      summary: Create a default category link
      description: Creates a link between a variation and a category that designates
        the category as the default category.
      operationId: postRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-post
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Category
      - Link
  /rest/items/{id}/variations/{variationId}/variation_default_categories/{plentyId}:
    delete:
      summary: Delete a default category link
      description: Deletes a link between a variation and a category that designates
        this category as the default category.
      operationId: deleteRestItemsVariationsVariationVariationDefaultCategoriesPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categoriesplentyid-delete
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Default
      - Category
      - Link
    get:
      summary: Gets a default category link
      description: Gets the default category linked to a variation for the specified
        client (store). The ID of the item, the ID of the variation and the ID of
        the client (store) must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategoriesPlenty
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categoriesplentyid-get
      parameters:
      - in: path
        name: id
      - in: path
        name: plentyId
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - S
      - Default
      - Category
      - Link
  /rest/markets/ebay/categories/{id}:
    get:
      summary: Get category
      description: Get category for given ID.
      operationId: getRestMarketsEbayCategories
      x-api-path-slug: restmarketsebaycategoriesid-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Category
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