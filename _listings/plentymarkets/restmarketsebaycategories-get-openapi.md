---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List categories
  description: Lists categories. By passing category ID as filter, only subcategories
    of that category will be returned. The marketplace ID filter is required.
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